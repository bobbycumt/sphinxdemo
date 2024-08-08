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

