# 积木分拣机
## 简介

使用[哪吒科学套件](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html)搭配[ELECFREAKS Interactive Coding Accessories Pack](https://shop.elecfreaks.com/products/elecfreaks-interactive-coding-accessories-pack)
来制作一台积木分拣机。

![](./images/neza-inventor-s-kit-case-71-01.png)

## 案例搭建

### 所需器材

[ELECFREAKS micro:bit Nezha 48 IN 1 Inventor's Kit ](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-nezha-48-in-1-inventors-kit-without-micro-bit-board)

[ELECFREAKS Interactive Coding Accessories Pack](https://shop.elecfreaks.com/products/elecfreaks-interactive-coding-accessories-pack)


### 结构搭建

零件清单

![](./images/neza-inventor-s-kit-case-71-02.png)

如图所示，进行结构搭建：

![](./images/neza-inventor-s-kit-step-71-01.png)

![](./images/neza-inventor-s-kit-step-71-02.png)

![](./images/neza-inventor-s-kit-step-71-03.png)

![](./images/neza-inventor-s-kit-step-71-04.png)

![](./images/neza-inventor-s-kit-step-71-05.png)

![](./images/neza-inventor-s-kit-step-71-06.png)

![](./images/neza-inventor-s-kit-step-71-07.png)

![](./images/neza-inventor-s-kit-step-71-08.png)

![](./images/neza-inventor-s-kit-step-71-09.png)

![](./images/neza-inventor-s-kit-step-71-10.png)

![](./images/neza-inventor-s-kit-step-71-11.png)

![](./images/neza-inventor-s-kit-step-71-12.png)

![](./images/neza-inventor-s-kit-step-71-13.png)

![](./images/neza-inventor-s-kit-step-71-14.png)

![](./images/neza-inventor-s-kit-step-71-15.png)

![](./images/neza-inventor-s-kit-step-71-16.png)

![](./images/neza-inventor-s-kit-step-71-17.png)

![](./images/neza-inventor-s-kit-step-71-18.png)

![](./images/neza-inventor-s-kit-step-71-19.png)

![](./images/neza-inventor-s-kit-step-71-20.png)

搭建完成：

![](./images/neza-inventor-s-kit-step-71-21.png)

### 连接示意图

如下图所示，将彩虹灯环连接到哪吒多功能扩展盒的J1端口，将颜色识别传感器连接到哪吒多功能扩展盒的IIC端口，将舵机连接到哪吒多功能扩展盒的S1接口。

![](./images/neza-inventor-s-kit-case-71-04.png)


## makecode编程

### 步骤 1
在MakeCode的代码抽屉中点击“扩展”。

![](./images/neza-inventor-s-kit-case-37-04.png)

为了对灯环进行编程，我们需要添加一个扩展库。在对话框中输入”PlanetX“，并点击搜索，点击下载这个代码库。

![](./images/neza-inventor-s-kit-case-37-05.png)

为了对哪吒扩展板进行编程，我们需要添加一个扩展库。在对话框中输入”Nezha“，并点击搜索，点击下载这个代码库。

![](./images/neza-inventor-s-kit-case-37-06.png)

*注意：*如果你得到一个提示说一些代码库因为不兼容的原因将被删除，你可以根据提示继续操作，或者在项目菜单栏里面新建一个项目。

### 步骤 2

### 如图所示编写程序

![](./images/neza-inventor-s-kit-case-71-06.png)

### 参考程序

请参考程序连接：[https://makecode.microbit.org/_3tkXK83pFDoH](https://makecode.microbit.org/_3tkXK83pFDoH)

你也可以通过以下网页直接下载程序，下载完成后即可开始运行程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_3tkXK83pFDoH" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  



### 结果
通过颜色传感器来分辨积木颜色并通过彩虹灯环显示出来，根据识别到的颜色将积木进行分类。

![](./images/neza-inventor-s-kit-case-71.gif)

