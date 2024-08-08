## analogWrite：模拟输出

将一个模拟数值写进Arduino引脚。这个操作可以用来控制**LED的亮度**，或者控制**电机的转速**。

**arduino uno**中，analogWrite()函数支持以下引脚:**<font color='red'>3, 5, 6, 9, 10, 11</font>** 。

在Arduino Mega控制其中,该函数支持引脚 2 – 13 和 44 – 46。

### 语法

```
analogWrite(pin, value)
```

### 参数

`pin`：被读取的模拟引脚号码
`value`：0到255之间

### 示例

```c++
analogWrite(3, 255);
```

