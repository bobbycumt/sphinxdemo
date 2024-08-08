## substring()：获得子串

获取 String 的子字符串。起始索引是包含的（相应的字符包含在子字符串中），但可选的结束索引是独占的（相应的字符不包含在子字符串中）。如果省略结束索引，则子字符串将继续到 String 的末尾。

### 语法

- ```arduino
  myString.substring(from)
  ```

- ```arduino
  myString.substring(from, to)
  ```

### 参数

- myString：类型的变量String
- from：开始子字符串的索引
- to（可选）：在子字符串之前结束的索引

### 返回

子字符串。

