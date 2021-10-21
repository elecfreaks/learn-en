# 定时喂养


##  简介
---
 
- 人工喂养动物是非常麻烦的，我们可以制作一个定时喂养装置。

##  功能
---
- 通过RTC计时模块进行计时，当达到特定时间时，则控制舵机转动进行投喂。

## 购买链接
---
- 1 x [microbit Smart Agriculture Kit]()

## 产品图片
---
![](./images/microbit-Smart-Agriculture-Kit-case-01-02.png)

## 硬件链接
---

将舵机连接到IOT:bit的P1端口，OLED显示屏连接到IOT:bit的IIC端口。

![](./images/microbit-Smart-Agriculture-Kit-case-11-03.png)

## 软件编程
---
在MakeCode的代码抽屉中点击“高级”，查看更多代码选项。

![](./images/microbit-Smart-Agriculture-Kit-case-01-04.png)

为了给microbit Smart City Kit编程，我们需要添加一个扩展库。在代码抽屉底部找到“扩展”，并点击它。这时会弹出一个对话框，搜索”iot-environment-kit“，然后点击下载这个代码库。

![](./images/microbit-Smart-Agriculture-Kit-case-01-05.png)

为了给舵机编程，我们需要添加一个扩展库。在代码抽屉底部找到“扩展”，并点击它。这时会弹出一个对话框，搜索”servo“，然后点击下载这个代码库。

![](./images/microbit-Smart-Agriculture-Kit-case-01-06.png)

*注意：*如果你得到一个提示说一些代码库因为不兼容的原因将被删除，你可以根据提示继续操作，或者在项目菜单栏里面新建一个项目。

## 程序
---

当开机时初始化OLED显示屏为128×64，初始化RTC时钟的初始时间，设置舵机转动到0度。

![](./images/microbit-Smart-Agriculture-Kit-case-11-07.png)

通过OLED显示屏显示当前秒数。

![](./images/microbit-Smart-Agriculture-Kit-case-11-08.png)

当秒数等于1时，舵机转动到90度，延迟5秒，再转动到0度。

![](./images/microbit-Smart-Agriculture-Kit-case-11-09.png)

请参考程序连接：[https://makecode.microbit.org/_RE7cgtJCJMFP](https://makecode.microbit.org/_RE7cgtJCJMFP)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_RE7cgtJCJMFP" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## 结果
---
- 自动投喂装置每分钟自动投喂一次食物。



