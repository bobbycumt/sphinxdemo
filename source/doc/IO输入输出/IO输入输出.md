



## pinMode：引脚模式设定
引脚模式设定，通常在setup函数里，三种引脚模式

> [!IMPORTANT]
>
> OUTPUT：输出模式
>
> INPUT：输入模式
>
> INPUT_PULLUP：输入上拉模式

```c++
void setup()
{
    //第一个参数是引脚号，第二个参数是模式
    pinMode(13, OUTPUT);
}
```
------

## digitalWrite：数字输出
将数字引脚写HIGH（高电平）或LOW（低电平）

### 语法

```
digitalWrite(pin, value)
```

### 参数

`pin`：引脚号码

`value`: [HIGH](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/high/) 或 [LOW](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/low/)

### 示例

```c++
digitalWrite(13, HIGH);//第一个参数是引脚号，第二个参数是高或低，也可以是1或0
```

------

## digitalRead：数字输入

读取数字引脚的 HIGH(高电平）或 LOW（低电平）。

### 语法

```
digitalRead(pin)
```

### 参数

`pin`：被读取的引脚号码

### 返回

0或1

### 示例

```C++
if(digitalRead(2)==1)
{
    digitalWrite(3,1);
}
```

------

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

------

## analogRead：模拟输入

本指令用于从Arduino的模拟输入引脚(A0-A5)读取数值。主要用于电位器、模拟光强度传感器、模拟声音传感器。数值范围为0-1023.

### 语法

```
analogRead(pin)
```

### 参数

`pin`：被读取的模拟引脚号码

### 返回值

0到1023之间的值

### 示例

```C++
int val = 0;           
 
void setup()
{
    //Arduino串口通讯初始化 
    Serial.begin(9600); 
}
 
void loop()
{
    //读取引脚A0输入信号
    val = analogRead(A0);   

    //将A0输入信号转换为0-1023之间的数值
    //并且通过串口监视器显示 
    Serial.println(val); 
}
```

