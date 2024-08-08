## byte：字节

byte类型变量可存储8位无符号数，其存储数值范围是 0 – 255。

byte类型变量在控制LED时显得格外有用，因为Arduino控制LED亮度或色彩时常常使用的数值是在0-255之间。

### 示例

```C++
byte b ;  // 创建byte类型变量b
 
void setup() {
  Serial.begin(9600); 
}
 
void loop() {
  b++;
  Serial.print("b = ");
  Serial.println(b); 
  /*
   * 将此程序编译并且上传Arduino后，通过串口监视器可以看到
   * 变量b的数值会从0开始逐1递增。在b的数值达到255时，
   * 当变量b再次执行b++操作后，变量b的数值将会复位到0，
   * 然后再次逐1递增。程序将会依次往复循环。
  */
}
```

