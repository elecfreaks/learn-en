# 案例01：便携指南针

## 目的
---
- 使用watch kit手表套件完成可穿戴便携式指南针带有多彩LED灯指示。

## 使用材料
---

- 1 x Watch kit 手表套件


## 背景知识
---

### 什么是指南针 
- [指南针](https://en.wikipedia.org/wiki/Compass)指南针，古代叫司南，主要组成部分是一根装在轴上的磁针，磁针在天然地磁场的作用下可以自由转动并保持在磁子午线的切线方向上，磁针的北极指向地理的南极，利用这一性能可以辨别方向。
### 指南针模块
- micro:bit主板带有指南针模块，可以完成指南针的功能。当指南针指向正北时返回值为0，顺时针增加到360，按不同的数值可以判断相关方向。

![](./images/2UMV4MA.png)



## 硬件连接图
---

如图所示，将灯环连接到power bit主板上。

![](./images/xLUYTkT.jpg)



## 软件
---
[微软makecode](https://makecode.microbit.org/#)

- 指南针模块每次使用时都需要初始化，初始化方式为一个小游戏，将点阵显示屏周围一圈点亮后，会显示一个笑脸即初始化完毕。

![](./images/V4wZAP1.png) ![](./images/EW3J71r.png)

## 编程
---
### 步骤 1
- 在MakeCode的代码抽屉中点击Advanced，查看更多代码选项。

![](./images/LjMR5IU.png)

- 为了给灯环模块编程，我们需要添加一个代码库。在代码抽屉底部找到“Add Package”，并点击它。这时会弹出一个对话框。搜索“nexpixel"，然后点击下载这个代码库。

![](./images/0u6UbMV.png)

注意：如果你得到一个提示说一些代码库因为不兼容的原因将被删除，你可以根据提示继续操作，或者在项目菜单栏里面新建一个项目。

### 步骤 2

- 在Basic中拖出一个on start积木块，在其中插入calibrate compass积木块。用于初始化指南针模块。

![](./images/watch_kit_case_01_01.png)

### 步骤 3
- 在forever 积木块中插入，将变量设置为指南针返回参数。
- 因为返回值范围为0-360，在灯环上有8个灯，所以将360等分为8份，北方向的范围为337到22，逐级递增。
- 当指向北方时，5号灯亮，主板同时发声提示。

![](./images/watch_kit_case_01_02.png)

### 程序
- 请参考程序连接：[https://makecode.microbit.org/_cj1EUmFJH6At](https://makecode.microbit.org/_cj1EUmFJH6At)

- 你也可以通过以下网页直接下载程序。

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_cj1EUmFJH6At" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---


## 结论
---
- 指向北方时5号灯亮红色，发出提示音。
![](./images/mSYW7Kg.gif)


## 思考
---


## 常见问题
---
问：每次使用方向不定？
答：指南针只是方向是大概，和每次校准结果有关。

## 相关阅读  
---

