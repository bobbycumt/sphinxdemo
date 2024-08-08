## char：字符型

char数据类型使用**1个字节**的内存来存储单个字符值。字符以[ASCII编码](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/ascii-code-table/)的形式存储。字符应写在单引号中，如: ‘A’。（char数据类型不能存储字符串。另外在Arduino编程中，由多个字符组成的字符串应使用双引号来表示，如：“ABC”。）

字符的[ASCII](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/ascii-code-table/)值可以用来作数学计算。如以下语句：

```C++
char asciiB = 'A'+ 1;
```

以上语句中，因为大写A的[ASCII](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/ascii-code-table/)值是65，所以运行结果是66，也就是大写B的[ASCII编码](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/ascii-code-table/)。

char数据类型是有符号的类型，这意味着它的编码为-128到127。

### 示例

```C++
char myChar = ‘A’;
char myChar = 65; // 两种声明结果都是相同的
```

