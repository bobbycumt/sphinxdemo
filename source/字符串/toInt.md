## toInt()：转整数

将有效的 String 转换为整数。输入 String 应以整数开头。如果 String 包含非整数，则该函数将停止执行转换。

### 示例

```C++
int a;
String s1="123";
a=s1.toInt();//返回整数123
String s2="123abc";
a=s2.toInt();//返回整数123
String s3="abc123";
a=s3.toInt();//返回整数0
String s4="12a3";
a=s4.toInt();//返回整数12
```

如果由于 String 不以整数开头而无法执行有效转换，则返回零。





