## Serial.readString()：读取字符串

函数从串行缓冲区读取字符到一个字符串中。如果超时，函数将终止。

### 示例

```C++
void setup() { 
    Serial.begin(9600); 
} 

void loop() { 
    Serial.println("Enter data:");
    while (Serial.available() == 0) {} // 等待数据可用
    String teststr = Serial.readString(); // 读取直到超时
    teststr.trim(); // 移除字符串末尾的任何空白字符
    if (teststr == "red") { 
        Serial.println("A primary color"); 
    } else { 
        Serial.println("Something else"); 
    } 
}
```

