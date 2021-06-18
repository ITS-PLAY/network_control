# 想法

加入每个相位的权重系数，用于计算特定方向的评级指标；加入最大最小周期时长约束；

加入相位差；



# 0章

 the main parameter is the time dimesion that determines how efficiently the avaiable roadway space is used by confilicting traffic streams.

# 2章

## 延误和饱和度关键指标

![image-20210616105650357](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616105650357.png)

(P22)

## 饱和度评价过程

![image-20210616110620964](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616110620964.png)

(P24)

## 交叉口名词的英语描述

![image-20210616111226197](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616111226197.png)

## 6个影响因素

![image-20210616111738906](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616111738906.png)

(P27)

## 优化的可选目标

![image-20210616140133461](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616140133461.png)

## 交叉口设计的流程

![image-20210616141630072](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616141630072.png)

(P30)

# 3章

## 到达流和离开流

![image-20210616143448846](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616143448846.png)

(P34)

## 车辆换算系数

![image-20210616144531248](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616144531248.png)

(P35)

## 评价时长的选择

![image-20210616155654609](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616155654609.png)

(P37)

## 基本饱和流率，实际饱和流率的考虑因素

​	基本饱和流率的调整（S~basic~），需考虑的环境因素：

​     1）天气条件；

​     2）路面条件；

​     3）交叉口环境，干扰因素。

​	

​	实际饱和流率（S~adj~）的调整因素（F~adj~）如下：

​    1）物理条件：

​           车道宽度、坡度、转弯半径、排队和消散空间；

​	2）交通流条件：

​			公交车站、停车站、行人；

​	3）控制条件：

​			绿灯时长、保护左转、允许左转、有行人的保护左转、有行人的右转、混合车道。

​	   S~adj~=S~basic~*f(F~adj~)

(P46-P72)

## 信号配时的考虑因素

​	信号配时参数包含：

​	1）相位组合；

​	2）周期结构：相位数和相序；

​	3）绿灯时长；

​	4）红灯时长；

​	5）黄灯时长；

​	6）全红时长；

​	（P75）

​	其他的配时参数根据需要，也可包含如下：

​	1）行人；

​	2）自行车；

​	3）公交运行；

​	4）信号协调；

​	5）特殊控制需求，例如交通感应相位或者公交优先信号；

​	6）排队控制；

​	7）需求管理；

​	8）控制设备；

​	9）控制软件。

​	（P85）

### 相位组合和周期结构

![image-20210616175225546](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616175225546.png)

### 相位组合的指导建议

![image-20210616175027634](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616175027634.png)

​	(P75-P76)



![image-20210616180521084](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210616180521084.png)

​	(P78)



![image-20210617091559724](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617091559724.png)

### 公交优先控制的三种渐进式方法

​	公交优先可以分为三类：

​	1）被动式优先。基于公交频率和速度，离线设计配时方案，适用于公交流量较大的场景；

​	2）主动式优先。采用优先相位绿灯延长，非优先相位红灯早断，专门插入优先相位等方式；

​							又可分为无条件的公交优先，有条件的公交优先（考虑乘客数量或者保证公交准点率 ）

​	3）自适应优先。减少通道整体延误和最大化乘客通行。

​	（P92)

### 方案选择式控制的优化方法（适用特殊事件）

![image-20210617112610726](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617112610726.png)

​	P(96)

### 实时自适应控制描述（适用多变的交通流）

​	![image-20210617135429826](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617135429826.png)

​	（P97）



### 感应式控制的最佳周期

​	![image-20210617142246529](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617142246529.png)

​	

# 4章

## 最小和最优的周期时长

![image-20210617161010634](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617161010634.png)

​	（P106）

## 周期时长与延误、通行能力关系

![image-20210617161120137](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617161120137.png)

​	（P107）



## 绿灯分配的方法

![image-20210617162441689](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617162441689.png)

​	（P108）

## 协调信号考虑的因素

![image-20210617165042252](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617165042252.png)

​	（P113）

## 评价指标

![image-20210617172705419](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617172705419.png)

​	（P115）

### 延误的计算

![image-20210617174129576](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617174129576.png)

​	（P122）

### 排队长度（排队远端）计算

![image-20210617180053993](C:\Users\lixiaohui\AppData\Roaming\Typora\typora-user-images\image-20210617180053993.png)



