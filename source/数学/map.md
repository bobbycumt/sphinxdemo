## map：等比映射

map()可以用来将某一数值从一个区间等比映射到一个新的区间。

### 语法

`map (x, in_min, in_max, out_min, out_max) `

### 参数

`x`： 要映射的值
`in_min`： 映射前区间最小值
`in_max`： 映射前区间最大值
`out_min`： 映射后区间最小值
`out_max`：映射后区间最大值

### 示例

```C++
void loop()
{
    int val = analogRead(0);
    val = map(val, 0, 1023, 0, 255);  //将变量val数值从 0 － 1023 区间映射到 0 － 255区间
    analogWrite(9, val);
}
```

