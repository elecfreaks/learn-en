# case 04 Smart Wardrobe

![](./images/1BOixPA.jpg)
## Goal
---


- Make an auto window.

## Materials
---

- 1 x Smart home Kit
- 1 x corrugated board

## Background
---
### What is an auto window ? 
-  Noise pollution is a common problem in our life. When the value of noise higher than 70dB, it is will impact our health. We will design a smart window and door using micro:bit.

### Auto window operation
- Using micro:bit detect wether the the value of noise higher than 70dB and control servo to closing the door and the window.

![](./images/g674G7D.png)

## Practical operation
---
Materials: corrugated board and cutter

![](./images/PuJE7uj.jpg)

Build as below picture：

Front side：

![](./images/sPzbv3R.jpg)

Back side：

![](./images/hvyJ9Ow.jpg)

Paste devices as below piture:

![](./images/oSZrVnY.jpg)


## Hardware connect
---
![](./images/hOlsKaR.png)






## Software
---
[makecode](https://makecode.microbit.org/#)

Edge Connector Data Sheet



## Programming
---
### Step 1
Go to MakeCode page, click Advanced in the code block and click on Extensions.

![](./images/2qCyzQ7.png)

We need to add a new codebase for programming of smart home. Finding “Add Package” in the bottom of code block and click it. Then a message box will show up, search “smart home"， and download this new codebase.

![](./images/QR2s7LD.png)

***Note：*** If there is a hint says some codebase will be deleted because of incompatibility. Don't worry. You could go ahead as the hint or build a new item in item menu bar.


### Step 2

Drag on start on from Basic, snap into servo write pin, set P1 to 0.


![](./images/cAwF1Yb.png)

### Step 3

Snap set item to into forever, assignment value of noise to noise variables.

![](./images/V2ptpb6.png)

### Step 4

If value of noise > 70dB, snap into servo write pin,set P1 to 0 and the window be closed.

![](./images/RGf9xF5.png)

### Step 5
If value of noise < 70dB，snap into servo write pin,set P1 to 100 and the window be opened.

![](./images/5VmbsGn.png)
### Programming

Make code：[https://makecode.microbit.org/_Trh6x75hYcAT](https://makecode.microbit.org/_Trh6x75hYcAT)

You also could directly download program visit website as below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Trh6x75hYcAT" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

## Result
---
micro:bit driving servo open the window when value of noise > 70dB.

Front side：
![](./images/2JsAZKA.jpg)

Back side：
![](./images/rGIkINB.jpg)

## Think
---
How to know wether open the window on room temperature.

## Questions
---


## More information   
---

