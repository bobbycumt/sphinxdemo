## bool / boolean：布尔型

bool为C++标准支持关键字，在arduino中兼容；boolean为arduino专用关键字，在编程中两种类型声明均可。

布尔型变量是有两种逻辑状态的变量，它包含两个值:[true](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/true-false/)（真）或 [false](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/true-false/)（假）。（每个布尔变量占用一个字节的内存。）

如果在表达式中使用了布尔型变量，那么将根据变量值的真假而赋予整型值1或0。要把一个整型变量转换成布尔型变量，如果该变量的整型值为0，则其布尔型值为假；反之如果整型值为非0，则其布尔型值为真。布尔型变量在运行时通常用做标志，比如进行逻辑测试以改变程序流程。

### 示例

```c++
boolean pushButton; // 创建布尔型变量
 
void setup() 
{
    pinMode(2, INPUT_PULLUP); //将引脚2设置为输入上拉模式
    pinMode(13, OUTPUT);      //将引脚13设置为输出模式
}
 
void loop() 
{
    pushButton = digitalRead(2); //读取引脚2电平状态并将其赋值给布尔变量

    if (pushButton)
    {          //根据布尔变量数值点亮或者熄灭LED
    	digitalWrite(13, HIGH); //布尔变量值为真（true）时点亮LED
    }
    else 
    {
    	digitalWrite(13, LOW);  //布尔变量值为假（false）时熄灭LED
    }
}
```
