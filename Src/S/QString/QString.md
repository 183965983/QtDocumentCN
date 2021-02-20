这里是文档翻译的模板，详情请见[贡献指南](https://github.com/QtDocumentCN/QtDocumentCN/blob/master/CONTRIBUTING.md)。

文档翻译的名词对照表可见[对照表](Comparison_Table.md)。

翻译文档结构为三层目录结构。

```markdown
# 类名
	## 公共成员类型
	## 公有成员函数
	## 成员类型文档
		### 类型1
		### 类型2
	## 成员函数文档
		### 函数1
		### 函数2
```



# QString

QString 类提供了一个Unicode字符组成的字符串。

|   属性 | 方法                |
| -----: | :------------------ |
| 头文件 | `#include<QString>` |
|  qmake | `QT+=core`          |

## 公共成员类型

| 类型    | 方法                                                         |
| ------- | ------------------------------------------------------------ |
| class   | **[Null](https://doc.qt.io/archives/qt-5.9/qstring-null.html)** |
| typedef | **[ConstIterator](https://doc.qt.io/archives/qt-5.9/qstring.html#ConstIterator-typedef)** |
| typedef | **[Iterator](https://doc.qt.io/archives/qt-5.9/qstring.html#Iterator-typedef)** |
| enum    | **[NormalizationForm](https://doc.qt.io/archives/qt-5.9/qstring.html#NormalizationForm-enum)** { NormalizationForm_D, NormalizationForm_C, NormalizationForm_KD, NormalizationForm_KC } |
| enum    | **[SectionFlag](https://doc.qt.io/archives/qt-5.9/qstring.html#SectionFlag-enum)** { SectionDefault, SectionSkipEmpty, SectionIncludeLeadingSep, SectionIncludeTrailingSep, SectionCaseInsensitiveSeps } |
| flags   | **[SectionFlags](https://doc.qt.io/archives/qt-5.9/qstring.html#SectionFlag-enum)** |
| enum    | **[SplitBehavior](https://doc.qt.io/archives/qt-5.9/qstring.html#SplitBehavior-enum)** { KeepEmptyParts, SkipEmptyParts } |
| typedef | **[const_iterator](https://doc.qt.io/archives/qt-5.9/qstring.html#const_iterator-typedef)** |
| typedef | **[const_pointer](https://doc.qt.io/archives/qt-5.9/qstring.html#const_pointer-typedef)** |
| typedef | **[const_reference](https://doc.qt.io/archives/qt-5.9/qstring.html#const_reference-typedef)** |
| typedef | **[const_reverse_iterator](https://doc.qt.io/archives/qt-5.9/qstring.html#const_reverse_iterator-typedef)** |
| typedef | **[difference_type](https://doc.qt.io/archives/qt-5.9/qstring.html#difference_type-typedef)** |
| typedef | **[iterator](https://doc.qt.io/archives/qt-5.9/qstring.html#iterator-typedefx)** |
| typedef | **[pointer](https://doc.qt.io/archives/qt-5.9/qstring.html#pointer-typedef)** |
| typedef | **[reference](https://doc.qt.io/archives/qt-5.9/qstring.html#reference-typedef)** |
| typedef | **[reverse_iterator](https://doc.qt.io/archives/qt-5.9/qstring.html#reverse_iterator-typedef)** |
| typedef | **[size_type](https://doc.qt.io/archives/qt-5.9/qstring.html#size_type-typedef)** |
| typedef | **[value_type](https://doc.qt.io/archives/qt-5.9/qstring.html#value_type-typedef)** |

## 公共成员函数

| 返回类型               | 函数名                                                       |
| ---------------------- | ------------------------------------------------------------ |
|                        | **[ QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString)**() |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-1)**(const QChar **unicode*, int *size* = -1) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-2)**(QChar *ch*) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-3)**(int *size*, QChar *ch*) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-4)**(QLatin1String *str*) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-5)**(const QString &*other*) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-6)**(QString &&*other*) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-7)**(const char **str*) |
|                        | **[QString](https://doc.qt.io/archives/qt-5.9/qstring.html#QString-8)**(const QByteArray &*ba*) |
|                        | **[~QString](https://doc.qt.io/archives/qt-5.9/qstring.html#dtor.QString)**() |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append)**(const QString &*str*) |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append-1)**(const QChar **str*, int *len*) |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append-2)**(QChar *ch*) |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append-3)**(const QStringRef &*reference*) |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append-4)**(QLatin1String *str*) |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append-5)**(const char **str*) |
| QString &              | **[append](https://doc.qt.io/archives/qt-5.9/qstring.html#append-6)**(const QByteArray &*ba*) |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg)**(const QString &*a*, int *fieldWidth* = 0, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-1)**(qulonglong *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-2)**(long *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-3)**(ulong *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-4)**(int *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-5)**(uint *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-6)**(short *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-7)**(ushort *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-8)**(double *a*, int *fieldWidth* = 0, char *format* = 'g', int *precision* = -1, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-9)**(char *a*, int *fieldWidth* = 0, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-10)**(QChar *a*, int *fieldWidth* = 0, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-11)**(qlonglong *a*, int *fieldWidth* = 0, int *base* = 10, QChar *fillChar* = QLatin1Char( ' ' )) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-12)**(const QString &*a1*, const QString &*a2*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-13)**(const QString &*a1*, const QString &*a2*, const QString &*a3*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-14)**(const QString &*a1*, const QString &*a2*, const QString &*a3*, const QString &*a4*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-15)**(const QString &*a1*, const QString &*a2*, const QString &*a3*, const QString &*a4*, const QString &*a5*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-16)**(const QString &*a1*, const QString &*a2*, const QString &*a3*, const QString &*a4*, const QString &*a5*, const QString &*a6*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-17)**(const QString &*a1*, const QString &*a2*, const QString &*a3*, const QString &*a4*, const QString &*a5*, const QString &*a6*, const QString &*a7*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-18)**(const QString &*a1*, const QString &*a2*, const QString &*a3*, const QString &*a4*, const QString &*a5*, const QString &*a6*, const QString &*a7*, const QString &*a8*) const |
| QString                | **[arg](https://doc.qt.io/archives/qt-5.9/qstring.html#arg-19)**(const QString &*a1*, const QString &*a2*, const QString &*a3*, const QString &*a4*, const QString &*a5*, const QString &*a6*, const QString &*a7*, const QString &*a8*, const QString &*a9*) const |
| const QChar            | **[at](https://doc.qt.io/archives/qt-5.9/qstring.html#at)**(int *position*) const |
| iterator               | **[begin](https://doc.qt.io/archives/qt-5.9/qstring.html#begin)**() |
| const_iterator         | **[begin](https://doc.qt.io/archives/qt-5.9/qstring.html#begin-1)**() const |
| int                    | **[capacity](https://doc.qt.io/archives/qt-5.9/qstring.html#capacity)**() const |
| const_iterator         | **[cbegin](https://doc.qt.io/archives/qt-5.9/qstring.html#cbegin)**() const |
| const_iterator         | **[cend](https://doc.qt.io/archives/qt-5.9/qstring.html#cend)**() const |
| void                   | **[chop](https://doc.qt.io/archives/qt-5.9/qstring.html#chop)**(int *n*) |
| void                   | **[clear](https://doc.qt.io/archives/qt-5.9/qstring.html#clear)**() |
| int                    | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare-1)**(QLatin1String *other*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare-2)**(const QString &*other*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare-5)**(const QStringRef &*ref*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| const_iterator         | **[constBegin](https://doc.qt.io/archives/qt-5.9/qstring.html#constBegin)**() const |
| const QChar *          | **[constData](https://doc.qt.io/archives/qt-5.9/qstring.html#constData)**() const |
| const_iterator         | **[constEnd](https://doc.qt.io/archives/qt-5.9/qstring.html#constEnd)**() const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains)**(const QString &*str*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-1)**(QChar *ch*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-2)**(QLatin1String *str*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-3)**(const QStringRef &*str*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-4)**(const QRegExp &*rx*) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-5)**(QRegExp &*rx*) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-6)**(const QRegularExpression &*re*) const |
| bool                   | **[contains](https://doc.qt.io/archives/qt-5.9/qstring.html#contains-7)**(const QRegularExpression &*re*, QRegularExpressionMatch **match*) const |
| int                    | **[count](https://doc.qt.io/archives/qt-5.9/qstring.html#count)**(const QString &*str*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[count](https://doc.qt.io/archives/qt-5.9/qstring.html#count-1)**(QChar *ch*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[count](https://doc.qt.io/archives/qt-5.9/qstring.html#count-2)**() const |
| int                    | **[count](https://doc.qt.io/archives/qt-5.9/qstring.html#count-3)**(const QStringRef &*str*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[count](https://doc.qt.io/archives/qt-5.9/qstring.html#count-4)**(const QRegExp &*rx*) const |
| int                    | **[count](https://doc.qt.io/archives/qt-5.9/qstring.html#count-5)**(const QRegularExpression &*re*) const |
| const_reverse_iterator | **[crbegin](https://doc.qt.io/archives/qt-5.9/qstring.html#crbegin)**() const |
| const_reverse_iterator | **[crend](https://doc.qt.io/archives/qt-5.9/qstring.html#crend)**() const |
| QChar *                | **[data](https://doc.qt.io/archives/qt-5.9/qstring.html#data)**() |
| const QChar *          | **[data](https://doc.qt.io/archives/qt-5.9/qstring.html#data-1)**() const |
| iterator               | **[end](https://doc.qt.io/archives/qt-5.9/qstring.html#end)**() |
| const_iterator         | **[end](https://doc.qt.io/archives/qt-5.9/qstring.html#end-1)**() const |
| bool                   | **[endsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#endsWith)**(const QString &*s*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[endsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#endsWith-1)**(const QStringRef &*s*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[endsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#endsWith-2)**(QLatin1String *s*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[endsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#endsWith-3)**(QChar *c*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| QString &              | **[fill](https://doc.qt.io/archives/qt-5.9/qstring.html#fill)**(QChar *ch*, int *size* = -1) |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf)**(const QString &*str*, int *from* = 0, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-1)**(QChar *ch*, int *from* = 0, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-2)**(QLatin1String *str*, int *from* = 0, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-3)**(const QStringRef &*str*, int *from* = 0, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-4)**(const QRegExp &*rx*, int *from* = 0) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-5)**(QRegExp &*rx*, int *from* = 0) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-6)**(const QRegularExpression &*re*, int *from* = 0) const |
| int                    | **[indexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#indexOf-7)**(const QRegularExpression &*re*, int *from*, QRegularExpressionMatch **rmatch*) const |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert)**(int *position*, const QString &*str*) |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert-1)**(int *position*, const QChar **unicode*, int *size*) |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert-2)**(int *position*, QChar *ch*) |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert-3)**(int *position*, const QStringRef &*str*) |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert-4)**(int *position*, QLatin1String *str*) |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert-5)**(int *position*, const char **str*) |
| QString &              | **[insert](https://doc.qt.io/archives/qt-5.9/qstring.html#insert-6)**(int *position*, const QByteArray &*str*) |
| bool                   | **[isEmpty](https://doc.qt.io/archives/qt-5.9/qstring.html#isEmpty)**() const |
| bool                   | **[isNull](https://doc.qt.io/archives/qt-5.9/qstring.html#isNull)**() const |
| bool                   | **[isRightToLeft](https://doc.qt.io/archives/qt-5.9/qstring.html#isRightToLeft)**() const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf)**(const QString &*str*, int *from* = -1, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-1)**(QChar *ch*, int *from* = -1, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-2)**(QLatin1String *str*, int *from* = -1, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-3)**(const QStringRef &*str*, int *from* = -1, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-4)**(const QRegExp &*rx*, int *from* = -1) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-5)**(QRegExp &*rx*, int *from* = -1) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-6)**(const QRegularExpression &*re*, int *from* = -1) const |
| int                    | **[lastIndexOf](https://doc.qt.io/archives/qt-5.9/qstring.html#lastIndexOf-7)**(const QRegularExpression &*re*, int *from*, QRegularExpressionMatch **rmatch*) const |
| QString                | **[left](https://doc.qt.io/archives/qt-5.9/qstring.html#left)**(int *n*) const |
| QString                | **[leftJustified](https://doc.qt.io/archives/qt-5.9/qstring.html#leftJustified)**(int *width*, QChar *fill* = QLatin1Char( ' ' ), bool *truncate* = false) const |
| QStringRef             | **[leftRef](https://doc.qt.io/archives/qt-5.9/qstring.html#leftRef)**(int *n*) const |
| int                    | **[length](https://doc.qt.io/archives/qt-5.9/qstring.html#length)**() const |
| int                    | **[localeAwareCompare](https://doc.qt.io/archives/qt-5.9/qstring.html#localeAwareCompare-1)**(const QString &*other*) const |
| int                    | **[localeAwareCompare](https://doc.qt.io/archives/qt-5.9/qstring.html#localeAwareCompare-2)**(const QStringRef &*other*) const |
| QString                | **[mid](https://doc.qt.io/archives/qt-5.9/qstring.html#mid)**(int *position*, int *n* = -1) const |
| QStringRef             | **[midRef](https://doc.qt.io/archives/qt-5.9/qstring.html#midRef)**(int *position*, int *n* = -1) const |
| QString                | **[normalized](https://doc.qt.io/archives/qt-5.9/qstring.html#normalized)**(NormalizationForm *mode*, QChar::UnicodeVersion *version* = QChar::Unicode_Unassigned) const |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend)**(const QString &*str*) |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend-1)**(const QChar **str*, int *len*) |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend-2)**(QChar *ch*) |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend-3)**(const QStringRef &*str*) |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend-4)**(QLatin1String *str*) |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend-5)**(const char **str*) |
| QString &              | **[prepend](https://doc.qt.io/archives/qt-5.9/qstring.html#prepend-6)**(const QByteArray &*ba*) |
| void                   | **[push_back](https://doc.qt.io/archives/qt-5.9/qstring.html#push_back)**(const QString &*other*) |
| void                   | **[push_back](https://doc.qt.io/archives/qt-5.9/qstring.html#push_back-1)**(QChar *ch*) |
| void                   | **[push_front](https://doc.qt.io/archives/qt-5.9/qstring.html#push_front)**(const QString &*other*) |
| void                   | **[push_front](https://doc.qt.io/archives/qt-5.9/qstring.html#push_front-1)**(QChar *ch*) |
| reverse_iterator       | **[rbegin](https://doc.qt.io/archives/qt-5.9/qstring.html#rbegin)**() |
| const_reverse_iterator | **[rbegin](https://doc.qt.io/archives/qt-5.9/qstring.html#rbegin-1)**() const |
| QString &              | **[remove](https://doc.qt.io/archives/qt-5.9/qstring.html#remove)**(int *position*, int *n*) |
| QString &              | **[remove](https://doc.qt.io/archives/qt-5.9/qstring.html#remove-1)**(QChar *ch*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[remove](https://doc.qt.io/archives/qt-5.9/qstring.html#remove-2)**(const QString &*str*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[remove](https://doc.qt.io/archives/qt-5.9/qstring.html#remove-3)**(const QRegExp &*rx*) |
| QString &              | **[remove](https://doc.qt.io/archives/qt-5.9/qstring.html#remove-4)**(const QRegularExpression &*re*) |
| reverse_iterator       | **[rend](https://doc.qt.io/archives/qt-5.9/qstring.html#rend)**() |
| const_reverse_iterator | **[rend](https://doc.qt.io/archives/qt-5.9/qstring.html#rend-1)**() const |
| QString                | **[repeated](https://doc.qt.io/archives/qt-5.9/qstring.html#repeated)**(int *times*) const |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace)**(int *position*, int *n*, const QString &*after*) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-1)**(int *position*, int *n*, const QChar **unicode*, int *size*) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-2)**(int *position*, int *n*, QChar *after*) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-3)**(QChar *before*, QChar *after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-4)**(const QChar **before*, int *blen*, const QChar **after*, int *alen*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-5)**(QLatin1String *before*, QLatin1String *after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-6)**(QLatin1String *before*, const QString &*after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-7)**(const QString &*before*, QLatin1String *after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-8)**(const QString &*before*, const QString &*after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-9)**(QChar *ch*, const QString &*after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-10)**(QChar *c*, QLatin1String *after*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-11)**(const QRegExp &*rx*, const QString &*after*) |
| QString &              | **[replace](https://doc.qt.io/archives/qt-5.9/qstring.html#replace-12)**(const QRegularExpression &*re*, const QString &*after*) |
| void                   | **[reserve](https://doc.qt.io/archives/qt-5.9/qstring.html#reserve)**(int *size*) |
| void                   | **[resize](https://doc.qt.io/archives/qt-5.9/qstring.html#resize)**(int *size*) |
| void                   | **[resize](https://doc.qt.io/archives/qt-5.9/qstring.html#resize-1)**(int *size*, QChar *fillChar*) |
| QString                | **[right](https://doc.qt.io/archives/qt-5.9/qstring.html#right)**(int *n*) const |
| QString                | **[rightJustified](https://doc.qt.io/archives/qt-5.9/qstring.html#rightJustified)**(int *width*, QChar *fill* = QLatin1Char( ' ' ), bool *truncate* = false) const |
| QStringRef             | **[rightRef](https://doc.qt.io/archives/qt-5.9/qstring.html#rightRef)**(int *n*) const |
| QString                | **[section](https://doc.qt.io/archives/qt-5.9/qstring.html#section)**(QChar *sep*, int *start*, int *end* = -1, SectionFlags *flags* = SectionDefault) const |
| QString                | **[section](https://doc.qt.io/archives/qt-5.9/qstring.html#section-1)**(const QString &*sep*, int *start*, int *end* = -1, SectionFlags *flags* = SectionDefault) const |
| QString                | **[section](https://doc.qt.io/archives/qt-5.9/qstring.html#section-2)**(const QRegExp &*reg*, int *start*, int *end* = -1, SectionFlags *flags* = SectionDefault) const |
| QString                | **[section](https://doc.qt.io/archives/qt-5.9/qstring.html#section-3)**(const QRegularExpression &*re*, int *start*, int *end* = -1, SectionFlags *flags* = SectionDefault) const |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum)**(int *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-1)**(ushort *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-2)**(short *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-3)**(uint *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-4)**(long *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-5)**(ulong *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-6)**(qlonglong *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-7)**(qulonglong *n*, int *base* = 10) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-8)**(float *n*, char *format* = 'g', int *precision* = 6) |
| QString &              | **[setNum](https://doc.qt.io/archives/qt-5.9/qstring.html#setNum-9)**(double *n*, char *format* = 'g', int *precision* = 6) |
| QString &              | **[setRawData](https://doc.qt.io/archives/qt-5.9/qstring.html#setRawData)**(const QChar **unicode*, int *size*) |
| QString &              | **[setUnicode](https://doc.qt.io/archives/qt-5.9/qstring.html#setUnicode)**(const QChar **unicode*, int *size*) |
| QString &              | **[setUtf16](https://doc.qt.io/archives/qt-5.9/qstring.html#setUtf16)**(const ushort **unicode*, int *size*) |
| QString                | **[simplified](https://doc.qt.io/archives/qt-5.9/qstring.html#simplified)**() const |
| int                    | **[size](https://doc.qt.io/archives/qt-5.9/qstring.html#size)**() const |
| QStringList            | **[split](https://doc.qt.io/archives/qt-5.9/qstring.html#split)**(const QString &*sep*, SplitBehavior *behavior* = KeepEmptyParts, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| QStringList            | **[split](https://doc.qt.io/archives/qt-5.9/qstring.html#split-1)**(QChar *sep*, SplitBehavior *behavior* = KeepEmptyParts, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| QStringList            | **[split](https://doc.qt.io/archives/qt-5.9/qstring.html#split-2)**(const QRegExp &*rx*, SplitBehavior *behavior* = KeepEmptyParts) const |
| QStringList            | **[split](https://doc.qt.io/archives/qt-5.9/qstring.html#split-3)**(const QRegularExpression &*re*, SplitBehavior *behavior* = KeepEmptyParts) const |
| QVector<QStringRef>    | **[splitRef](https://doc.qt.io/archives/qt-5.9/qstring.html#splitRef)**(const QString &*sep*, SplitBehavior *behavior* = KeepEmptyParts, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| QVector<QStringRef>    | **[splitRef](https://doc.qt.io/archives/qt-5.9/qstring.html#splitRef-1)**(QChar *sep*, SplitBehavior *behavior* = KeepEmptyParts, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| QVector<QStringRef>    | **[splitRef](https://doc.qt.io/archives/qt-5.9/qstring.html#splitRef-2)**(const QRegExp &*rx*, SplitBehavior *behavior* = KeepEmptyParts) const |
| QVector<QStringRef>    | **[splitRef](https://doc.qt.io/archives/qt-5.9/qstring.html#splitRef-3)**(const QRegularExpression &*re*, SplitBehavior *behavior* = KeepEmptyParts) const |
| void                   | **[squeeze](https://doc.qt.io/archives/qt-5.9/qstring.html#squeeze)**() |
| bool                   | **[startsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#startsWith)**(const QString &*s*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[startsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#startsWith-1)**(const QStringRef &*s*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[startsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#startsWith-2)**(QLatin1String *s*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| bool                   | **[startsWith](https://doc.qt.io/archives/qt-5.9/qstring.html#startsWith-3)**(QChar *c*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) const |
| void                   | **[swap](https://doc.qt.io/archives/qt-5.9/qstring.html#swap)**(QString &*other*) |
| CFStringRef            | **[toCFString](https://doc.qt.io/archives/qt-5.9/qstring.html#toCFString)**() const |
| QString                | **[toCaseFolded](https://doc.qt.io/archives/qt-5.9/qstring.html#toCaseFolded)**() const |
| double                 | **[toDouble](https://doc.qt.io/archives/qt-5.9/qstring.html#toDouble)**(bool **ok* = Q_NULLPTR) const |
| float                  | **[toFloat](https://doc.qt.io/archives/qt-5.9/qstring.html#toFloat)**(bool **ok* = Q_NULLPTR) const |
| QString                | **[toHtmlEscaped](https://doc.qt.io/archives/qt-5.9/qstring.html#toHtmlEscaped)**() const |
| int                    | **[toInt](https://doc.qt.io/archives/qt-5.9/qstring.html#toInt)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| QByteArray             | **[toLatin1](https://doc.qt.io/archives/qt-5.9/qstring.html#toLatin1)**() const |
| QByteArray             | **[toLocal8Bit](https://doc.qt.io/archives/qt-5.9/qstring.html#toLocal8Bit)**() const |
| long                   | **[toLong](https://doc.qt.io/archives/qt-5.9/qstring.html#toLong)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| qlonglong              | **[toLongLong](https://doc.qt.io/archives/qt-5.9/qstring.html#toLongLong)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| QString                | **[toLower](https://doc.qt.io/archives/qt-5.9/qstring.html#toLower)**() const |
| NSString *             | **[toNSString](https://doc.qt.io/archives/qt-5.9/qstring.html#toNSString)**() const |
| short                  | **[toShort](https://doc.qt.io/archives/qt-5.9/qstring.html#toShort)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| std::string            | **[toStdString](https://doc.qt.io/archives/qt-5.9/qstring.html#toStdString)**() const |
| std::u16string         | **[toStdU16String](https://doc.qt.io/archives/qt-5.9/qstring.html#toStdU16String)**() const |
| std::u32string         | **[toStdU32String](https://doc.qt.io/archives/qt-5.9/qstring.html#toStdU32String)**() const |
| std::wstring           | **[toStdWString](https://doc.qt.io/archives/qt-5.9/qstring.html#toStdWString)**() const |
| uint                   | **[toUInt](https://doc.qt.io/archives/qt-5.9/qstring.html#toUInt)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| ulong                  | **[toULong](https://doc.qt.io/archives/qt-5.9/qstring.html#toULong)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| qulonglong             | **[toULongLong](https://doc.qt.io/archives/qt-5.9/qstring.html#toULongLong)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| ushort                 | **[toUShort](https://doc.qt.io/archives/qt-5.9/qstring.html#toUShort)**(bool **ok* = Q_NULLPTR, int *base* = 10) const |
| QVector<uint>          | **[toUcs4](https://doc.qt.io/archives/qt-5.9/qstring.html#toUcs4)**() const |
| QString                | **[toUpper](https://doc.qt.io/archives/qt-5.9/qstring.html#toUpper)**() const |
| QByteArray             | **[toUtf8](https://doc.qt.io/archives/qt-5.9/qstring.html#toUtf8)**() const |
| int                    | **[toWCharArray](https://doc.qt.io/archives/qt-5.9/qstring.html#toWCharArray)**(wchar_t **array*) const |
| QString                | **[trimmed](https://doc.qt.io/archives/qt-5.9/qstring.html#trimmed)**() const |
| void                   | **[truncate](https://doc.qt.io/archives/qt-5.9/qstring.html#truncate)**(int *position*) |
| const QChar *          | **[unicode](https://doc.qt.io/archives/qt-5.9/qstring.html#unicode)**() const |
| const ushort *         | **[utf16](https://doc.qt.io/archives/qt-5.9/qstring.html#utf16)**() const |
| bool                   | **[operator!=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-not-eq)**(QLatin1String *other*) const |
| bool                   | **[operator!=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-not-eq-1)**(const char **other*) const |
| bool                   | **[operator!=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-not-eq-2)**(const QByteArray &*other*) const |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq)**(const QString &*other*) |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq-2)**(QChar *ch*) |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq-3)**(const QStringRef &*str*) |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq-4)**(QLatin1String *str*) |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq-5)**(const char **str*) |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq-6)**(const QByteArray &*ba*) |
| QString &              | **[operator+=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-eq-7)**(char *ch*) |
| bool                   | **[operator<](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt)**(QLatin1String *other*) const |
| bool                   | **[operator<](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-1)**(const char **other*) const |
| bool                   | **[operator<](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-2)**(const QByteArray &*other*) const |
| bool                   | **[operator<=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-eq)**(QLatin1String *other*) const |
| bool                   | **[operator<=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-eq-1)**(const char **other*) const |
| bool                   | **[operator<=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-eq-2)**(const QByteArray &*other*) const |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq)**(const QString &*other*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-1)**(QChar *ch*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-2)**(QLatin1String *str*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-3)**(QString &&*other*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-4)**(const char **str*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-5)**(const QByteArray &*ba*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-6)**(char *ch*) |
| QString &              | **[operator=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-7)**(*const Null &*) |
| bool                   | **[operator==](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-eq)**(QLatin1String *other*) const |
| bool                   | **[operator==](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-eq-1)**(const char **other*) const |
| bool                   | **[operator==](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-eq-2)**(const QByteArray &*other*) const |
| bool                   | **[operator>](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt)**(QLatin1String *other*) const |
| bool                   | **[operator>](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-1)**(const char **other*) const |
| bool                   | **[operator>](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-2)**(const QByteArray &*other*) const |
| bool                   | **[operator>=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-eq)**(QLatin1String *other*) const |
| bool                   | **[operator>=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-eq-1)**(const char **other*) const |
| bool                   | **[operator>=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-eq-2)**(const QByteArray &*other*) const |
| QCharRef               | **[operator[\]](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-5b-5d)**(int *position*) |
| const QChar            | **[operator[\]](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-5b-5d-1)**(int *position*) const |
| const QChar            | **[operator[\]](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-5b-5d-2)**(uint *position*) const |
| QCharRef               | **[operator[\]](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-5b-5d-3)**(uint *position*) |

## 静态成员函数

| 返回类型 | 函数名                                                       |
| -------- | ------------------------------------------------------------ |
| QString  | **[asprintf](https://doc.qt.io/archives/qt-5.9/qstring.html#asprintf)**(const char **cformat*, *...*) |
| int      | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare)**(const QString &*s1*, const QString &*s2*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| int      | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare-3)**(const QString &*s1*, QLatin1String *s2*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| int      | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare-4)**(QLatin1String *s1*, const QString &*s2*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| int      | **[compare](https://doc.qt.io/archives/qt-5.9/qstring.html#compare-6)**(const QString &*s1*, const QStringRef &*s2*, Qt::CaseSensitivity *cs* = Qt::CaseSensitive) |
| QString  | **[fromCFString](https://doc.qt.io/archives/qt-5.9/qstring.html#fromCFString)**(CFStringRef *string*) |
| QString  | **[fromLatin1](https://doc.qt.io/archives/qt-5.9/qstring.html#fromLatin1)**(const char **str*, int *size* = -1) |
| QString  | **[fromLatin1](https://doc.qt.io/archives/qt-5.9/qstring.html#fromLatin1-1)**(const QByteArray &*str*) |
| QString  | **[fromLocal8Bit](https://doc.qt.io/archives/qt-5.9/qstring.html#fromLocal8Bit)**(const char **str*, int *size* = -1) |
| QString  | **[fromLocal8Bit](https://doc.qt.io/archives/qt-5.9/qstring.html#fromLocal8Bit-1)**(const QByteArray &*str*) |
| QString  | **[fromNSString](https://doc.qt.io/archives/qt-5.9/qstring.html#fromNSString)**(const NSString **string*) |
| QString  | **[fromRawData](https://doc.qt.io/archives/qt-5.9/qstring.html#fromRawData)**(const QChar **unicode*, int *size*) |
| QString  | **[fromStdString](https://doc.qt.io/archives/qt-5.9/qstring.html#fromStdString)**(const std::string &*str*) |
| QString  | **[fromStdU16String](https://doc.qt.io/archives/qt-5.9/qstring.html#fromStdU16String)**(const std::u16string &*str*) |
| QString  | **[fromStdU32String](https://doc.qt.io/archives/qt-5.9/qstring.html#fromStdU32String)**(const std::u32string &*str*) |
| QString  | **[fromStdWString](https://doc.qt.io/archives/qt-5.9/qstring.html#fromStdWString)**(const std::wstring &*str*) |
| QString  | **[fromUcs4](https://doc.qt.io/archives/qt-5.9/qstring.html#fromUcs4)**(const uint **unicode*, int *size* = -1) |
| QString  | **[fromUcs4](https://doc.qt.io/archives/qt-5.9/qstring.html#fromUcs4-1)**(const char32_t **str*, int *size* = -1) |
| QString  | **[fromUtf8](https://doc.qt.io/archives/qt-5.9/qstring.html#fromUtf8)**(const char **str*, int *size* = -1) |
| QString  | **[fromUtf8](https://doc.qt.io/archives/qt-5.9/qstring.html#fromUtf8-1)**(const QByteArray &*str*) |
| QString  | **[fromUtf16](https://doc.qt.io/archives/qt-5.9/qstring.html#fromUtf16)**(const ushort **unicode*, int *size* = -1) |
| QString  | **[fromUtf16](https://doc.qt.io/archives/qt-5.9/qstring.html#fromUtf16-1)**(const char16_t **str*, int *size* = -1) |
| QString  | **[fromWCharArray](https://doc.qt.io/archives/qt-5.9/qstring.html#fromWCharArray)**(const wchar_t **string*, int *size* = -1) |
| int      | **[localeAwareCompare](https://doc.qt.io/archives/qt-5.9/qstring.html#localeAwareCompare)**(const QString &*s1*, const QString &*s2*) |
| int      | **[localeAwareCompare](https://doc.qt.io/archives/qt-5.9/qstring.html#localeAwareCompare-3)**(const QString &*s1*, const QStringRef &*s2*) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number)**(long *n*, int *base* = 10) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number-1)**(uint *n*, int *base* = 10) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number-2)**(int *n*, int *base* = 10) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number-3)**(ulong *n*, int *base* = 10) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number-4)**(qlonglong *n*, int *base* = 10) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number-5)**(qulonglong *n*, int *base* = 10) |
| QString  | **[number](https://doc.qt.io/archives/qt-5.9/qstring.html#number-6)**(double *n*, char *format* = 'g', int *precision* = 6) |
| QString  | **[vasprintf](https://doc.qt.io/archives/qt-5.9/qstring.html#vasprintf)**(const char **cformat*, va_list *ap*) |

## 相关的非成员

| bool          | **[operator!=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-not-eq-3)**(const QString &*s1*, const QString &*s2*) |
| ------------- | ------------------------------------------------------------ |
| bool          | **[operator!=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-not-eq-4)**(const char **s1*, const QString &*s2*) |
| const QString | **[operator+](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b)**(const QString &*s1*, const QString &*s2*) |
| const QString | **[operator+](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-1)**(const QString &*s1*, const char **s2*) |
| const QString | **[operator+](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-2)**(const char **s1*, const QString &*s2*) |
| const QString | **[operator+](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-3)**(const QString &*s*, char *ch*) |
| const QString | **[operator+](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-2b-4)**(char *ch*, const QString &*s*) |
| bool          | **[operator<](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-3)**(const char **s1*, const QString &*s2*) |
| QDataStream & | **[operator<<](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-lt)**(QDataStream &*stream*, const QString &*string*) |
| bool          | **[operator<=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-eq-3)**(const QString &*s1*, const QString &*s2*) |
| bool          | **[operator<=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-lt-eq-4)**(const char **s1*, const QString &*s2*) |
| bool          | **[operator==](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-eq-eq-3)**(const char **s1*, const QString &*s2*) |
| bool          | **[operator>](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-3)**(const QString &*s1*, const QString &*s2*) |
| bool          | **[operator>](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-4)**(const char **s1*, const QString &*s2*) |
| bool          | **[operator>=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-eq-3)**(const QString &*s1*, const QString &*s2*) |
| bool          | **[operator>=](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-eq-4)**(const char **s1*, const QString &*s2*) |
| QDataStream & | **[operator>>](https://doc.qt.io/archives/qt-5.9/qstring.html#operator-gt-gt)**(QDataStream &*stream*, QString &*string*) |

## 宏

|      | **[ QStringLiteral](https://doc.qt.io/archives/qt-5.9/qstring.html#QStringLiteral)**(*str*) |
| ---- | ------------------------------------------------------------ |
|      | **[QT_NO_CAST_FROM_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_NO_CAST_FROM_ASCII)** |
|      | **[QT_NO_CAST_TO_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_NO_CAST_TO_ASCII)** |
|      | **[QT_RESTRICTED_CAST_FROM_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_RESTRICTED_CAST_FROM_ASCII)** |

## 详细介绍

QString 类提供了一个Unicode字符组成的字符串

QString存储一个含有多个16比特QChar的字符串，其中每个QChar都相当于一个Unicode4.0字符。（对应值大于65535的Unicode字符会用一对代理来表示，也就是说，两个连续的QChar）。

Unicode是支持绝大多数今天的书写系统的国际通用标准。是US-ASCII(ANSI X3.4-1986)、Latin-1(ISO 8859-1)的超集，所有US_ASCII、Latin-1的字符都存放在相同的编码位置。

在后台，QString使用隐式共享（写时拷贝）方案来减少内存使用，避免数据的频繁拷贝。这同时也减少了存放16比特字符而不是8比特字符的固有开销。

除QString之外，Qt同时也提供了QByteArray类来存放原始字节数据或传统的以’\0‘结尾的字符串。在多数情况下，QString会是最优选择。它完全依赖于Qt-API以及Unicode支持保证了应用的可移植性。QByteArray一般在两个场景中更优：存储二进制原始数据时，内存紧张时（比如在嵌入式系统中）。

### 初始化一个字符串

初始化一个QString的一种方法是直接将const char* 传给它的构造函数，举个例子，下方的代码创建了一个大小为5，包含数据“Hello”的QString:

```c++
QString str = "Hello";
```

QString调用fromUtf8()函数将const char*数据转换为了Unicode数据。

在所有接受const char\*参数的QString函数中，const char\*类型都被编译成了UTF-8编码，标准C风格，'\0'结尾的字符串。以“0”作为const char\*参数是合法的。

你也可以以QChar表格的形式提供字符串数据：

```c++
static const QChar data[4] = { 0x0055, 0x006e, 0x10e3, 0x03a3 };
QString str(data, 4);
```

QString执行诗词QChar数据的深拷贝，所以你可以在之后改变他而不引起其他影响。（如果为了性能需求，你不想对字符数据进行深拷贝，使用QString::fromRawData()代替。）

另一个方法是使用resize()设置字符串的大小，然后依次初始化每个字符数据。QString与C++数组一样，使用从“0”开始的索引， 使用operator[]来访问指定索引位置的字符。在非const字符串中，operator[]()返回一个可以在赋值运算中被当作左值的字符索引。如下：

```c++
QString str;
str.resize(4);

str[0] = QChar('U');
str[1] = QChar('n');
str[2] = QChar(0x10e3);
str[3] = QChar(0x03a3);
```

对于只读访问，可以使用at()函数：

```C++
QString str;

for (int i = 0; i < str.size(); ++i) {
    if (str.at(i) >= QChar('a') && str.at(i) <= QChar('f'))
        qDebug() << "Found character in range [a-f]";
}
```

at()函数比operator\[]()更快，因为它不进行深拷贝。也可以使用left()，right()，或mid()函数来一次性地提取多个字符。

一个QString中可以含有'\0'字符（QChar::Null）。size()函数始终会返回整个字符串的长度，包含其中的'\0'字符。

### 操作字符串数据

QString提供了如下的基本函数来修改字符数据：append()，prepend()，insert()，replace()，和remove()。比如：

```c++
QString str = "and";
str.prepend("rock ");     // str == "rock and"
str.append(" roll");        // str == "rock and roll"
str.replace(5, 3, "&");   // str == "rock & roll"
```

如果你在逐步建立一个QString，并且提前预估其将包含多少个字符。

## 属性文档

### currentLoop : const int

xxx

**存取函数**

| 返回类型 | 函数名                  |
| :------: | :---------------------- |
|   int    | **currentLoop**() const |

**通知信号**

| 返回类型 | 函数名                                                       |
| :------: | :----------------------------------------------------------- |
|   void   | [currentLoopChanged](A/QAbstractAnimation/QAbstractAnimation.md#signal-void-qabstractanimationcurrentloopchangedint-currentloop)(int *currentLoop*) |


----------

### currentTime : int

xxx

**存取函数**

| 返回类型 | 函数名                        |
| :------: | :---------------------------- |
|   int    | **currentTime**() const       |
|   void   | **setCurrentTime**(int msecs) |



## 成员类型文档

### enum **QAbstractSocket**::BindFlag | flags **QAbstractSocket**::BindMode

这里填该类型详细信息。

----

### XXX

这里填该类型详细信息。



## 成员函数文档

### QAbstractAnimation::**QAbstractAnimation**([QObject](O/QObject/QObject.md) *\*parent* = Q_NULLPTR)

构造 QAbstractAnimation 基类，并将 `parent` 参数传递给 [QObject](O/QObject/QObject.md) 的构造函数。

**另请参阅：**[QVariantAnimation](V/QVariantAnimation/QVariantAnimation.md) 和 [QAnimationGroup](A/QAnimationGroup/QAnimationGroup.md)

----------

###  **[signal]** void QAbstractAnimation::**currentLoopChanged**(int *currentLoop*)

每当当前循环发生变化时，[QAbstractAnimation](A/QAbstractAnimation/QAbstractAnimation.md) 会发射该信号。`currentLoop` 为当前循环。

**注意：** 属性 `currentLoop` 的通知信号。

**另请参阅：** [currentLoop](A/QAbstractAnimation/QAbstractAnimation.md#currentloop--const-int)() 和 [loopCount](A/QAbstractAnimation/QAbstractAnimation.md#loopcount--int)()。



## 宏文档

### QStringLiteral(str)

这个宏根据str字符串中的文字在编译时为QString生成数据。用这种方式建立的QString是不耗费资源的，并且生成的字符串数据是被存储在编译对象文件的只读区域中。

如果你有这样一段代码：

```c++
// hasAttribute takes a QString argument
if (node.hasAttribute("http-contents-length")) //...
```

一个临时QString会被建立，然后作为参数传递给hasAttribute函数。这么做运行开销可能非常大，不仅要分配内存，还要将数据拷贝或转换为QString的内部编码。

这样的开销可以通过使用QStringLiteral来避免。

```c++
if (node.hasAttribute(QStringLiteral(u"http-contents-length"))) //...
```

这样，QString的内部数据会在编译时生成，在运行时，不会发生转换或内存分配。

使用QStringLiteral来替代C++中的双引号字符串将显著提升建立那些在编译时数据已知的QString实例的速度。

**提示：**在字符串被传递给可直接接受QLatin1String，并在重载中避免将其转换为QString的函数时QLatin1String仍然比QStringLiteral效率更高。比如，QString::operator==()就可以直接对QLatin1String进行比较:

```C++
if (attribute.name() == QLatin1String("http-contents-length")) //...
```

**提示：**一些编译器在遇到包含非US-ASCII字符的字符串时，进行字符串编码时会发生bug，此时，确保你在你的字符串前添加了“u”前缀，在其它情况下，也可以这么做。

**另请参阅：** [QByteArrayLiteral](https://doc.qt.io/archives/qt-5.9/qbytearray.html#QByteArrayLiteral).

### QT_NO_CAST_FROM_ASCII

禁止从8比特字符串(char*)到Unicode QString的自动转换。

**另请参阅：** [QT_NO_CAST_TO_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_NO_CAST_TO_ASCII), [QT_RESTRICTED_CAST_FROM_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_RESTRICTED_CAST_FROM_ASCII), 和 [QT_NO_CAST_FROM_BYTEARRAY](https://doc.qt.io/archives/qt-5.9/qbytearray.html#QT_NO_CAST_FROM_BYTEARRAY).

### QT_NO_CAST_TO_ASCII

禁止QString到8比特字符串(char*)的自动转换。

**另请参阅：**[QT_NO_CAST_FROM_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_NO_CAST_FROM_ASCII), [QT_RESTRICTED_CAST_FROM_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_RESTRICTED_CAST_FROM_ASCII), 和[QT_NO_CAST_FROM_BYTEARRAY](https://doc.qt.io/archives/qt-5.9/qbytearray.html#QT_NO_CAST_FROM_BYTEARRAY).

### QT_RESTRICTED_CAST_FROM_ASCII

定义此宏来禁止绝大多数的从文字和8比特数据到Unicode QString的自动转换，但是运行使用QChar(char)和QString(const char(&ch))[N]构造函数，并且QString::operator=(const char(&ch)[N])赋值运算符提供了QT_NO_CAST_FROM_ASCII的大多数类型安全优点，但不需要用户使用QLatin1Char，QLatin1String或类似字符来包装字符和字符串。 

**另请参阅：**[QT_NO_CAST_FROM_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_NO_CAST_FROM_ASCII) 和 [QT_NO_CAST_TO_ASCII](https://doc.qt.io/archives/qt-5.9/qstring.html#QT_NO_CAST_TO_ASCII).