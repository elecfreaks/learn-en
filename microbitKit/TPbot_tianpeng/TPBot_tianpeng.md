# 钮扣电池扩展板（power:bit）

## 简介
---

power:bit纽扣电池板是一种最小尺寸的微型扩展板。它能够给micro:bit主板供电，并且板载蜂鸣器，通过排针引出了P1、P2、GND、3V接口。可以与我们的亚克力表带和主板搭配使用。

## 特性 
---

- 由两个3V的CR2025锂电池供电。
- 板载蜂鸣器，蜂鸣器由P0口控制。
- 通过排针引出P1、P2、3V、GND引脚。 
- 可以搭配亚克力表带和micro:bit主板使用。

## 参数
---
项目 | 参数 
:-: | :-: 
品名|power:bit
版本号|V1.6
SKU| EF03409
工作电压|2.7~3.3V
蜂鸣器|支持
尺寸|42x52mm
净重|10.7g

### 外型与定位尺寸
![](./images/BQCpLVu.png)
## 引脚接口框图
![](./images/ONnPnR7.png)

## 主要功能模块介绍  
---  

### 电源开关  

I档打开电源，O档关闭电源。

### 1x4排针接口

![](./images/9uskWP9.png)

从排针引出P1、P2、3V、GND引脚，可以扩展使用。

### 两个CR2025电池座

![](./images/RkOmiZc.png)

可以便捷插入2025电池（3V锂锰扣式电池）供电

### 蜂鸣器  

![](./images/eNtjso8.png)

蜂鸣器由P0口控制，能够播放音乐。

## 快速上手  
---  

### 硬件连接  


通过五个螺丝丁将micro:bit主板和power:bit固定连接起来，并将两个3V的2025电池装入power:bit扩展板上电池座中。当开关拨动到I档时，2025电池给micro：bit主板和power:bit主板供电，拨动到O档时2025电池不供电。


### 软件编程  

打开makecode，编写程序micro：bit主板点阵屏显示爱心闪烁图案。
程序代码链接：[https://makecode.microbit.org/_MP28fbDmUMfz](https://makecode.microbit.org/_MP28fbDmUMfz)

你也能通过下列窗口直接下载代码

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_MP28fbDmUMfz" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### 结果  

micro：bit主板点阵显示爱心闪烁图案。

## 常见问题
