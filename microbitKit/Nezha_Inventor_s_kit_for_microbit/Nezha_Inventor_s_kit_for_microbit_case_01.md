# 机械虾

## 简介
使用[哪吒科学套件](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html)制作一只机械虾。

![](./images/neza-inventor-s-kit-case-37-01.png)

## 快速上手


### 所需器材

[哪吒科学套件](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html)

### 结构搭建

零件清单

![](./images/neza-inventor-s-kit-case-37-02.png)

如图所示，进行结构搭建：

![](./images/neza-inventor-s-kit-step-37-01.png)

![](./images/neza-inventor-s-kit-step-37-02.png)

![](./images/neza-inventor-s-kit-step-37-03.png)

![](./images/neza-inventor-s-kit-step-37-04.png)

![](./images/neza-inventor-s-kit-step-37-05.png)

![](./images/neza-inventor-s-kit-step-37-06.png)

![](./images/neza-inventor-s-kit-step-37-07.png)

![](./images/neza-inventor-s-kit-step-37-08.png)

![](./images/neza-inventor-s-kit-step-37-09.png)

![](./images/neza-inventor-s-kit-step-37-10.png)

![](./images/neza-inventor-s-kit-step-37-11.png)

![](./images/neza-inventor-s-kit-step-37-12.png)

![](./images/neza-inventor-s-kit-step-37-13.png)

![](./images/neza-inventor-s-kit-step-37-14.png)

![](./images/neza-inventor-s-kit-step-37-15.png)

![](./images/neza-inventor-s-kit-step-37-16.png)

![](./images/neza-inventor-s-kit-step-37-17.png)

![](./images/neza-inventor-s-kit-step-37-18.png)

![](./images/neza-inventor-s-kit-step-37-19.png)

![](./images/neza-inventor-s-kit-step-37-20.png)

![](./images/neza-inventor-s-kit-step-37-21.png)

![](./images/neza-inventor-s-kit-step-37-22.png)

![](./images/neza-inventor-s-kit-step-37-23.png)

![](./images/neza-inventor-s-kit-step-37-24.png)

![](./images/neza-inventor-s-kit-step-37-25.png)

![](./images/neza-inventor-s-kit-step-37-26.png)

![](./images/neza-inventor-s-kit-step-37-27.png)

![](./images/neza-inventor-s-kit-step-37-28.png)

![](./images/neza-inventor-s-kit-step-37-29.png)

![](./images/neza-inventor-s-kit-step-37-30.png)

![](./images/neza-inventor-s-kit-step-37-31.png)

![](./images/neza-inventor-s-kit-step-37-32.png)

![](./images/neza-inventor-s-kit-step-37-33.png)

### 连接示意图

如下图所示，将[超声波传感器](https://www.elecfreaks.com/planetx-ultrasonic.html)连接到[哪吒扩展板](https://www.elecfreaks.com/nezha-breakout-board.html)的J1端口、[舵机](https://www.elecfreaks.com/geekservo-2kg-360-degrees-compatible-with-lego.html)连接到[哪吒扩展板](https://www.elecfreaks.com/nezha-breakout-board.html)的S1端口，两个[电机](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html)分别连接到[哪吒扩展板](https://www.elecfreaks.com/nezha-breakout-board.html)的M1和M4端口。

![](./images/neza-inventor-s-kit-case-37-03.png)


## makecode编程



### 步骤 1
在MakeCode的代码抽屉中点击“扩展”。

![](./images/neza-inventor-s-kit-case-37-04.png)

为了对[超声波传感器](https://www.elecfreaks.com/planetx-ultrasonic.html)进行编程，我们需要添加一个扩展库。在对话框中输入”PlanetX“，并点击搜索，点击下载这个代码库。

![](./images/neza-inventor-s-kit-case-37-05.png)

为了对[哪吒扩展板](https://www.elecfreaks.com/nezha-breakout-board.html)进行编程，我们需要添加一个扩展库。在对话框中输入”Nezha“，并点击搜索，点击下载这个代码库。

![](./images/neza-inventor-s-kit-case-37-06.png)

*注意：*如果你得到一个提示说一些代码库因为不兼容的原因将被删除，你可以根据提示继续操作，或者在项目菜单栏里面新建一个项目。

### 步骤 2
### 如图所示编写程序

![](./images/neza-inventor-s-kit-case-37-07.png)


### 参考程序
请参考程序连接：[https://makecode.microbit.org/_iscUF8CzzYMd](https://makecode.microbit.org/_iscUF8CzzYMd)

你也可以通过以下网页直接下载程序，下载完成后即可开始运行程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_iscUF8CzzYMd" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### 结果

当电源接通后，机械虾向前移动并摆动大鳌，当遇到障碍物时，则自动转向。

