# AI摄像头控制吸管机械手



![](./images/straw-manipulator-26.gif)



### 简介

这节课我们需要用到AI摄像头和吸管机械手套件，根据AI摄像头识别不同颜色的小球做出不同的手势。

恩孚科技独立研发的AI摄像头可以实现人脸识别、小球识别、卡片识别、巡线识别、颜色识别和特征学习的功能。

关于AI摄像头更为详细的内容请参考：[AI摄像头相关文档](https://www.elecfreaks.com/learn-cn/microbitplanetX/ai/index.html)

### 所需材料

![](./images/straw-manipulator-08-1.png)

### 组装步骤


一、吸管机械手组装
吸管机械手的组装步骤请参考：[吸管机械手](./How-to-use-the-microbit-to-control-the-straw-manipulator.md)

二、AI摄像头组装

1、首先使用3颗黑销插入孔壁圈上并将15孔梁安装到黑销上面，如图所示：

![](./images/straw-manipulator-27.png)

2、将13孔梁以及黑销按如图所示安装：

![](./images/straw-manipulator-28.png)

3、将H型孔壁按如图所示安装：

![](./images/straw-manipulator-29.png)

4、将AI摄像头和RJ11转杜邦线按如图所示连接，注意：RJ11连接悟空扩展板的连接顺序如图所示：

![](./images/straw-manipulator-30.png)

### 开始编程

micro:bit编程是使用 [Makecode](https://makecode.microbit.org) 编程平台，关于添加悟空扩展库和编程方法，参考上一篇案例文档：[吸管机械手](https://www.elecfreaks.com/learn-cn/microbitKit/straw-manipulator/How-to-use-the-microbit-to-control-the-straw-manipulator.html)。

![](./images/straw-manipulator-18.png)

### 初始化

本教程所使用的初始化状态是：0度代表“手指”完全伸展，180度代表“手指”弯曲，所以，在开始正式编程之前要将舵机角度调整到0度。将单摆臂取下，使用 [Makecode](https://makecode.microbit.org) 编程如下程序代码，同时也可以直接下载下方程序。

![](./images/straw-manipulator-17.png)

程序代码：

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_azoXDPMYE35F" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div> 



将调整好后的舵机安装上单摆臂，就可以运行下方的程序代码，当然您也可以发挥自己的创造力，做出不同动作的“手舞”。



### 简单示例



![](./images/straw-manipulator-2-5.png)



参考程序链接：[AI摄像头控制机械手](https://makecode.microbit.org/_4qKFUwW2k6jV)

同时，也可以从直接运行下方编程积木块：

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_4qKFUwW2k6jV" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div> 



### 常见问题



吸管机械手使用的是180度舵机，所以控制舵机积木块的数值范围是：0~180。下载编程好的积木块代码到micro:bit后，打开悟空扩展板的电源开关，关于[悟空扩展板](https://www.elecfreaks.com/learn-en/microbitExtensionModule/wukong.html)的详细使用内容请参考其相关文档。
