# QString

QString 类提供了一个Unicode字符组成的字符串

QString存储一个含有多个16比特QChar的字符串，其中每个QChar都相当于一个Unicode4.0字符。（对应值大于65535的Unicode字符会用一对代理来表示，也就是说，两个连续的QChar）。

Unicode是支持绝大多数今天的书写系统的国际通用标准。是US-ASCII(ANSI X3.4-1986)、Latin-1(ISO 8859-1)的超集，所有US_ASCII、Latin-1的字符都存放在相同的编码位置。

在后台，QString使用隐式共享（写时拷贝）方案来减少内存使用，避免数据的频繁拷贝。这同时也减少了存放16比特字符而不是8比特字符的固有开销。

除QString之外，Qt同时也提供了QByteArray类来存放原始字节数据或传统的以’\0‘结尾的字符串。在多数情况下，QString会是最优选择。它完全依赖于Qt-API以及Unicode支持保证了应用的可移植性。QByteArray一般在两个场景中更优：存储二进制原始数据时，内存紧张时（比如在嵌入式系统中）。

## 初始化一个字符串

初始化一个QString的一种方法是直接将const char* 传给它的构造函数，举个例子，下方的代码创建了一个大小为5，包含数据“Hello”的QString:



QString调用fromUtf8()函数将const char*数据转换为了Unicode数据。

在所有接受const char*参数的QString函数中



### QStringLiteral(str)

这个宏根据str字符串中的文字在编译时为QString生成数据。用这种方式建立的QString是不耗费资源的，并且生成的字符串数据是被存储在编译对象文件的只读区域中。

如果你有这样一段代码：



一个临时QString会被建立，然后作为参数传递给hasAttribute函数。这么做运行开销可能非常大，不仅要分配内存，还要将数据拷贝或转换为QString的内部编码。

这样的开销可以通过使用QStringLiteral来避免。



这样，QString的内部数据会在编译时生成，在运行时，不会发生转换或内存分配。

使用QStringLiteral来替代C++中的双引号字符串将显著提升建立那些在编译时数据已知的QString实例的速度。

**提示：**在字符串被传递给可直接接受QLatin1String，并在重载中避免将其转换为QString的函数时QLatin1String仍然比QStringLiteral效率更高。比如，QString::operator==()就可以直接对QLatin1String进行比较:



**提示：**一些编译器在遇到包含非US-ASCII字符的字符串时，进行字符串编码时会发生bug，此时，确保你在你的字符串前添加了“u”前缀，在其它情况下，也可以这么做。



### QT_NO_CAST_FROM_ASCII

禁止从8比特字符串(char*)到Unicode QString的自动转换。



### QT_NO_CAST_TO_ASCII

禁止QString到8比特字符串(char*)的自动转换。



### QT_RESTRICTED_CAST_FROM_ASCII

定义此宏来禁止绝大多数的从文字和8比特数据到Unicode QString的自动转换，但是运行使用QChar(char)和QString(const char(&ch))[N]构造函数，并且QString::operator=(const char(&ch)[N])赋值运算符提供了QT_NO_CAST_FROM_ASCII的大多数类型安全优点，但不需要用户使用QLatin1Char，QLatin1String或类似字符来包装字符和字符串。 

