## digitalRead：数字输入

读取数字引脚的 HIGH(高电平）或 LOW（低电平）。

### 语法

```
digitalRead(pin)
```

### 参数

`pin`：被读取的引脚号码

### 返回

0或1

### 示例

```C++
if(digitalRead(2)==1)
{
    digitalWrite(3,1);
}
```

