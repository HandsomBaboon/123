spart1
（2）、（4）均为溢出错误
（7）出现精度误差
part2
)Method of complements In mathematics and computing, 
the method of complements is a technique used to 
subtract one number from another using
only addition of positive numbers. 

2)Byte字节（港澳台作位元组，英语：Byte），通常用作计算机信息计量单位，
不分数据类型。[1][2] 一个字节代表八个比特（港澳台作位元，英语：Bit）
3)Integer (computer science)In computer science, 
an integer is a datum of integral data type, a data
type that represents some range of
mathematical integers.


4) Floating-point arithmetic         In computing, 
floating-point arithmetic (FP) is arithmetic 
using formulaic representation of real 
numbers as an approximation so as
to support a trade-off between 
range and precision.
仔细阅读” Method of complements”的内容，你将注意到nines‘ complement in
the decimal 和 ones’ complement in binary 等概念.
1)请证明：二进制的负数（two‘s complement of X）等于 X 的 ones，
complement ＋ 1（即，X每位求反加1）
两个正数相加，就是他们补码的和。两个正数相减，由于减数转换成了补码，还是只要补码相加就行。
这样在硬件设计的时候，只用加法器就可以实现了，简化设计。
补码是在计算机内存中的存放的形式，第一个数字表示符号位，0正1负。
整数补码是其本身，负数补码是其绝对值的补码除了符号位以外的二进制数取反加1


2)Int8_t x = - 017; 请用8进制描述变量 x。
在c中017即(017)8 阅读维基百科” Two‘s complement”的内容，
特别是Sign extension小节内容。x=357（8）

1)C程序：int8_t x = -0x1f; int y = x; 请用16进制描述变量 x 和 y，并说明 int
y = x 的计算过程
。x=0xffffffe1,-0x1f转为十进制是-31，
2)请用数学证明，为什么可以这么计算。
x = -0x1f，转换为十进制数为-31.而-31的原码表示为1000 0000 0000 0000 0000 0000 0001 1111
，最高位为符号位（1为负数，0为非负数）。保持原码符号位不变，其余为取反后再加1即可得到其补码表示
1111 1111 1111 1111 1111 1111 1110 0001，然后把该二进制数转换为十六进制可得到0xffffffe1。
阅读维基百科” Floating point”的内容，
1)NaN 是什么？NaN（Not a Number，非数）是计算机科学中
数值数据类型的一类值，表示未定义或不可表示的值。
常在浮点数运算中使用 
