## pinMode：引脚模式设定
引脚模式设定，通常在setup函数里，三种引脚模式

> [!IMPORTANT]
>
> OUTPUT：输出模式
>
> INPUT：输入模式
>
> INPUT_PULLUP：输入上拉模式

```c++
void setup()
{
    //第一个参数是引脚号，第二个参数是模式
    pinMode(13, OUTPUT);
}
```
