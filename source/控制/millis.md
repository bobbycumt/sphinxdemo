## millis()：获取Arduino开机后运行的时间

millis函数可以用来获取Arduino开机后运行的时间长度，该时间长度单位是毫秒,最长可记录接近50天左右的时间。如果超出记录时间上限，记录将从0重新开始。

### 返回值

Arduino开机后运行的时间长度，此时间数值以毫秒为单位（返回值类型：[无符号长整型](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/unsigned-long/)）

### 注意：

millis函数的返回值为[无符号长整型](http://www.taichi-maker.com/homepage/reference-index/arduino-code-reference/unsigned-long/)数据, 如果将该数值与整型数据或其它数据类型进行运算，运行结果将产生错误。

### 示例程序-1

以下实例程序将通过串口监视器输出程序的运行时间

```C++
unsigned long time;
 
void setup(){
  Serial.begin(9600);
}
void loop(){
  Serial.print("Arduino has been running this sketch for ");
  time = millis();
  //输出程序运行时间
  Serial.print(time);
  Serial.println(" milliseconds.");
  delay(1000);
}
```

### 示例程序-2

```C++
/* 
 *  millisBlink
 * 本示例程序使用millis()函数控制Arduino开发板内置LED的点亮和熄灭。
*/
unsigned long previousBlinkTime;
int blinkInterval = 1000; //LED闪烁时间间隔
bool toggle;
 
void setup() {
  pinMode(LED_BUILTIN, OUTPUT); 
  Serial.begin(9600);
}
 
void loop() {  
  unsigned long currentMillis = millis(); // 获取当前时间
  millisBlink(currentMillis);
 
  /* 由于使用millis()函数控制LED闪烁，所以loop函数中没有delay。
   * 于是我们可以在loop函数中流畅的执行其他操作。
  */
 
}
 
void millisBlink(unsigned long currentTime) { 
  //检查是否到达时间间隔
  if (currentTime - previousBlinkTime >= blinkInterval) {    //如果时间间隔达到了
    toggle = (toggle == 1) ? 0 : 1;    
    digitalWrite(LED_BUILTIN, toggle);                       //执行闪烁LED操作
    
    previousBlinkTime = currentTime;  // 将检查时间复位   
    
    Serial.print(F("toggle = "));Serial.println(toggle);          
  }  else if (currentTime - previousBlinkTime <= 0) {   // 如果millis时间溢出
    previousBlinkTime = currentTime;
  }
}
```

