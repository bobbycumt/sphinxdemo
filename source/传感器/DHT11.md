## 温湿度传感器DHT11

安装扩展库**DHT sensor library**

### 对象声明和初始化

```c++
#include "DHT.h"	//头文件
DHT dht(2, DHT11);	//声明DHT类型的对象，类型与头文件名称相同，对象命名为dht，自行起名
void setup() 
{
    //串口打印按需使用
    Serial.begin(9600);
    Serial.println(F("DHT11 test!"));
	//使能传感器
    dht.begin();	
}
```

### 读取数据

```C++
//读取湿度，可以使用浮点型，也可以使用整型
float h = dht.readHumidity();
//读取温度，可以使用浮点型，也可以使用整型
float t = dht.readTemperature();
//注意读取间隔需大于等于2s
```

