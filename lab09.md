自顶向下：将复杂的大问题分解为相对简单的小问题，找出每个问题的关键、重点所在，然
后用精确的思维定性、定量地去描述问题。其核心本质是”分解”。 
逐步求精：将现实问题经过几次抽象（细化）处理，最后到求解域中只是一些简单的算法描
述和算法实现问题。即将系统功能按层次进行分解，每一层不断将功能细化，到最后一层都
是功能单一、简单易实现的模块。
通过观察，我发现大多数的洗衣机都有如下的特点：
1.选择洗衣模式： 对应水位， 注水时间
2.注水，水位计计水位
3.浸泡，计时器计时
4.电机转动，左 3 次， 右 3 次
5.排水，水位计计水位
6.电机转动（脱水）
7.结束， 关闭电源
下面给出这个程序的伪代码的实现：
READ 你是一个用户
REPEAT 注水
UNTIL 达到注水需求
timer 注水完成
REPEAT 浸泡
UNTIL timer.timeout()
timer.setTimeout(20)
WHILE (!timer.timeout()) 
rotate
rotate
ENDWHILE
WHILE (水位 ！= 0) 
排水 
ENDWHILE
timer.setTimeout(20) 
WHILE (!timer.timeout()) 
rotate
ENDWHILE 
其中上式rotate代表滚筒的转动
而timer代表对相应的时间进行计时


