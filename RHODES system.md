# RHODES的算法框架

​	四个层次：

​	1）network loading problem；

​        数据采集的时间间隔为周、日级。					

​		利用网络流的随机分配方法。然后将分配得到的路网OD和流量作为先验信息，根据实时数据计算后验值。

​	2）network flow control problem；

​		数据采集的时间间隔为若干分钟级。

​		包含两个方面：**状态估计**和**流控制**；

​    	其中，状态估计主要是不断更新流量估计值和预测曲线；

​				流控制用于确定大致（approximate)的相位和绿灯方案。分为两部分，一个称为节点间的通行能力分配(capacity allocation)，主要计算相位差和绿信比； 另一个称为节点的网络协调(network coordination)，主要确定相位和大致的绿灯时长；

​               ![image-20210618181522966](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210618181522966.png)

​               在流控制方面，主要采用REALBAND（基于决策树）算法，解决区域层面的车队冲突问题。

​               其中，决策树的每个节点代表车队的冲突，分支代表给某个车队的优先通行权或者某个车队被拆分；算法   更新的时间窗口的长短 或者 评价指标的上限（upper bound，如延误、停车次数），决定了决策树延伸到叶节点的终止条件。

​               另外，车队的概念，参考如下：

​               ![image-20210618182242848](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210618182242848.png)

​	3）intersection control problem；

​		 数据采集的时间间隔为1分钟级。

​		 用于确定合适(appropriate)的相序和相位方案。分为两个方面：一个称为交叉口的signal scheduling。主要确定交叉口的信号组合；另一个称为交叉口的intersection dispatching。主要微调当前信号绿灯时长，延长或缩短绿灯时长。

​	4）traffic signal actuation problem；

​         用于提供配时下发的接口（interface）



# 不同控制系统的演进过程

1）fixed-time plan;

2）on-line plan selection with off-line plan generation;

3）on-line plan selection and/or plane generation;

4）on-line timing;