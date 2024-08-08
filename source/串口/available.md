## Serial.available()：有数据到达

available() 函数可用于检查设备是否接收到数据。

```C++
void loop() 
{
  while (Serial.available())
  {                      // 当串口接收到信息后
    String serialData = Serial.readString();    // 将接收到的信息使用readString()存储于serialData变量
  }
}
```

