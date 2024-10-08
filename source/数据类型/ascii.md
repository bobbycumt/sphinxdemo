## ASCII码

ASCII（American Standard Code for Information Interchange，美国信息互换标准代码，ASCII）是基于拉丁字母的一套电脑编码系统。它主要用于显示现代英语和其他西欧语言。它是现今最通用的单字节编码系统，并等同于国际标准ISO/IEC 646。

ASCII码大致可以分作三部分组成。

### 第1部分：非打印控制字符

ASCII表上的数字0–31分配给了控制字符，用于控制像打印机等一些外围设备。例如，12代表换页/新页功能。此命令指示打印机跳到下一页的开头。当您查看或打印文档时这些字符不会显示出来（详参ASCII码表中0-31）

| 2进制    | 10进制 | 16进制 | 缩写/字符                   | 解释         |
| -------- | ------ | ------ | --------------------------- | ------------ |
| 00000000 | 0      | 00     | NUL(null)                   | 空字符       |
| 00000001 | 1      | 01     | SOH(start of headling)      | 标题开始     |
| 00000010 | 2      | 02     | STX (start of text)         | 正文开始     |
| 00000011 | 3      | 03     | ETX (end of text)           | 正文结束     |
| 00000100 | 4      | 04     | EOT (end of transmission)   | 传输结束     |
| 00000101 | 5      | 05     | ENQ (enquiry)               | 请求         |
| 00000110 | 6      | 06     | ACK (acknowledge)           | 收到通知     |
| 00000111 | 7      | 07     | BEL (bell)                  | 响铃         |
| 00001000 | 8      | 08     | BS (backspace)              | 退格         |
| 00001001 | 9      | 09     | HT (horizontal tab)         | 水平制表符   |
| 00001010 | 10     | 0A     | LF (NL line feed, new line) | 换行符       |
| 00001011 | 11     | 0B     | VT (vertical tab)           | 垂直制表符   |
| 00001100 | 12     | 0C     | FF (NP form feed, new page) | 换页键       |
| 00001101 | 13     | 0D     | CR (carriage return)        | 回车键       |
| 00001110 | 14     | 0E     | SO (shift out)              | 不用切换     |
| 00001111 | 15     | 0F     | SI (shift in)               | 启用切换     |
| 00010000 | 16     | 10     | DLE (data link escape)      | 数据链路转义 |
| 00010001 | 17     | 11     | DC1 (device control 1)      | 设备控制1    |
| 00010010 | 18     | 12     | DC2 (device control 2)      | 设备控制2    |
| 00010011 | 19     | 13     | DC3 (device control 3)      | 设备控制3    |
| 00010100 | 20     | 14     | DC4 (device control 4)      | 设备控制4    |
| 00010101 | 21     | 15     | NAK (negative acknowledge)  | 拒绝接收     |
| 00010110 | 22     | 16     | SYN (synchronous idle)      | 同步空闲     |
| 00010111 | 23     | 17     | ETB (end of trans. block)   | 传输块结束   |
| 00011000 | 24     | 18     | CAN (cancel)                | 取消         |
| 00011001 | 25     | 19     | EM (end of medium)          | 介质中断     |
| 00011010 | 26     | 1A     | SUB (substitute)            | 替补         |
| 00011011 | 27     | 1B     | ESC (escape)                | 溢出         |
| 00011100 | 28     | 1C     | FS (file separator)         | 文件分割符   |
| 00011101 | 29     | 1D     | GS (group separator)        | 分组符       |
| 00011110 | 30     | 1E     | RS (record separator)       | 记录分离符   |
| 00011111 | 31     | 1F     | US (unit separator)         | 单元分隔符   |

### 第2部分：打印字符

数字 32–126 分配给了能在键盘上找到的字符，当您查看或打印文档时这些字符将会显示出来。如数字49代表 字符’1’。（详参ASCII码表中32-127）

| 2进制    | 10进制 | 16进制 | 缩写/字符    | 解释 |
| -------- | ------ | ------ | ------------ | ---- |
| 00100000 | 32     | 20     | (space)      | 空格 |
| 00100001 | 33     | 21     | !            |      |
| 00100010 | 34     | 22     | “            |      |
| 00100011 | 35     | 23     | #            |      |
| 00100100 | 36     | 24     | $            |      |
| 00100101 | 37     | 25     | %            |      |
| 00100110 | 38     | 26     | &            |      |
| 00100111 | 39     | 27     | ‘            |      |
| 00101000 | 40     | 28     | (            |      |
| 00101001 | 41     | 29     | )            |      |
| 00101010 | 42     | 2A     | *            |      |
| 00101011 | 43     | 2B     | +            |      |
| 00101100 | 44     | 2C     | ,            |      |
| 00101101 | 45     | 2D     | –            |      |
| 00101110 | 46     | 2E     | .            |      |
| 00101111 | 47     | 2F     | /            |      |
| 00110000 | 48     | 30     | 0            |      |
| 00110001 | 49     | 31     | 1            |      |
| 00110010 | 50     | 32     | 2            |      |
| 00110011 | 51     | 33     | 3            |      |
| 00110100 | 52     | 34     | 4            |      |
| 00110101 | 53     | 35     | 5            |      |
| 00110110 | 54     | 36     | 6            |      |
| 00110111 | 55     | 37     | 7            |      |
| 00111000 | 56     | 38     | 8            |      |
| 00111001 | 57     | 39     | 9            |      |
| 00111010 | 58     | 3A     | :            |      |
| 00111011 | 59     | 3B     | ;            |      |
| 00111100 | 60     | 3C     | <            |      |
| 00111101 | 61     | 3D     | =            |      |
| 00111110 | 62     | 3E     | >            |      |
| 00111111 | 63     | 3F     | ?            |      |
| 01000000 | 64     | 40     | @            |      |
| 01000001 | 65     | 41     | A            |      |
| 01000010 | 66     | 42     | B            |      |
| 01000011 | 67     | 43     | C            |      |
| 01000100 | 68     | 44     | D            |      |
| 01000101 | 69     | 45     | E            |      |
| 01000110 | 70     | 46     | F            |      |
| 01000111 | 71     | 47     | G            |      |
| 01001000 | 72     | 48     | H            |      |
| 01001001 | 73     | 49     | I            |      |
| 01001010 | 74     | 4A     | J            |      |
| 01001011 | 75     | 4B     | K            |      |
| 01001100 | 76     | 4C     | L            |      |
| 01001101 | 77     | 4D     | M            |      |
| 01001110 | 78     | 4E     | N            |      |
| 01001111 | 79     | 4F     | O            |      |
| 01010000 | 80     | 50     | P            |      |
| 01010001 | 81     | 51     | Q            |      |
| 01010010 | 82     | 52     | R            |      |
| 01010011 | 83     | 53     | S            |      |
| 01010100 | 84     | 54     | T            |      |
| 01010101 | 85     | 55     | U            |      |
| 01010110 | 86     | 56     | V            |      |
| 01010111 | 87     | 57     | W            |      |
| 01011000 | 88     | 58     | X            |      |
| 01011001 | 89     | 59     | Y            |      |
| 01011010 | 90     | 5A     | Z            |      |
| 01011011 | 91     | 5B     | [            |      |
| 01011100 | 92     | 5C     | \            |      |
| 01011101 | 93     | 5D     | ]            |      |
| 01011110 | 94     | 5E     | ^            |      |
| 01011111 | 95     | 5F     | _            |      |
| 01100000 | 96     | 60     | `            |      |
| 01100001 | 97     | 61     | a            |      |
| 01100010 | 98     | 62     | b            |      |
| 01100011 | 99     | 63     | c            |      |
| 01100100 | 100    | 64     | d            |      |
| 01100101 | 101    | 65     | e            |      |
| 01100110 | 102    | 66     | f            |      |
| 01100111 | 103    | 67     | g            |      |
| 01101000 | 104    | 68     | h            |      |
| 01101001 | 105    | 69     | i            |      |
| 01101010 | 106    | 6A     | j            |      |
| 01101011 | 107    | 6B     | k            |      |
| 01101100 | 108    | 6C     | l            |      |
| 01101101 | 109    | 6D     | m            |      |
| 01101110 | 110    | 6E     | n            |      |
| 01101111 | 111    | 6F     | o            |      |
| 01110000 | 112    | 70     | p            |      |
| 01110001 | 113    | 71     | q            |      |
| 01110010 | 114    | 72     | r            |      |
| 01110011 | 115    | 73     | s            |      |
| 01110100 | 116    | 74     | t            |      |
| 01110101 | 117    | 75     | u            |      |
| 01110110 | 118    | 76     | v            |      |
| 01110111 | 119    | 77     | w            |      |
| 01111000 | 120    | 78     | x            |      |
| 01111001 | 121    | 79     | y            |      |
| 01111010 | 122    | 7A     | z            |      |
| 01111011 | 123    | 7B     | {            |      |
| 01111100 | 124    | 7C     | \|           |      |
| 01111101 | 125    | 7D     | }            |      |
| 01111110 | 126    | 7E     | ~            |      |
| 01111111 | 127    | 7F     | DEL (delete) | 删除 |

### 第3部分：扩展打印字符

扩展的ASCII字符满足了对更多字符的需求。扩展的ASCII包含ASCII中已有的128个字符（数字0–32显示在下图中），又增加了128个字符，总共是256个。即使有了这些更多的字符，许多语言还是包含无法压缩到256个字符中的符号。因此，出现了一些ASCII的变体来囊括地区性字符和符号。例如，许多软件程序把ASCII表（又称作ISO8859-1）用于北美、西欧、澳大利亚和非洲的语言。

