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

