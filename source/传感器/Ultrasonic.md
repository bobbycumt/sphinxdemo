## 超声波传感器

安装扩展库Ultrasonic

### 对象声明

```C++
#include <Ultrasonic.h>   //头文件
/*对象类型为Ultrasonic，与头文件名称相同，对象名称自定义
2个参数，第一个参数为trig连接的引脚号，第二个参数为echo连接的引脚号*/
Ultrasonic ultrasonic(12, 13);  

void setup()
{
    
}
```

### 距离读取

```c++
/*ultrasonic.read()为读取函数，有返回值，需要赋值给变量
distance为前面已经声明过的变量*/
distance = ultrasonic.read();
```

