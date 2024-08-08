## delay()：毫秒延时

delay()函数可用于暂停程序运行。暂停时间可以由delay()函数的参数进行控制，单位是毫秒（1秒钟＝1000毫秒）。

### 示例

```C++
void loop()
{
  digitalWrite(ledPin, HIGH);   // 点亮LED
  delay(1000);                  // 等待一秒钟（1000毫秒）
  digitalWrite(ledPin, LOW);    // 熄灭LED
  delay(1000);                  // 等待一秒钟（1000毫秒）
}
```

