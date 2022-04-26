# Lesson 06 Self-lock Switch 

 ![](./images/ogadD6b.jpg)  

## Introduction
---
Self-lock switch is a kind of common button switch. When we press the button for the first time, the switch is connected and remains that status, which is called “self-lock”. When we press the button for the second time, the switch is disconnected. At the same time, the button will bounce back to its initial place. In this experiment, we are going to use self-lock switch to control LED light.

## Component List

---
### Hardware：
- 1 x micro:bit Board
- 1 x Micro-B USB Cable
- 1 x microbit Breadboard Adapter
- 1 x Transparent Breadboard - 83 * 55 mm
- 1 x Self-lock Switch
- 1 x LED
- 1 x 100 Ohm Resistors
- n x Breadborad jumper wire 65pcs pack

****Tips: If you want all components above, you may need Elecfreaks micro:bit Starter Kit.****

![](./images/W4tseua.jpg)

## Major Components Introduction

---
### Self-lock Switch

Self-lock switch normally means switch with built-in mechanical lock function. Press down the switch and then release, it will not fully bounce up because it is locked. You have to press it again, then it will be unlocked and fully bounce up. This is the so-called Self-lock Switch. It is widely used to earlier televisions and monitors with function of directly completely power off.

![](./images/hareBrE.jpg)

Note: This kind of self-lock switch contains two groups of double-throw switch. In this experiment, we use a group only. So we cut down the common footer of a group.

## Experimental Procedure
---
### Hardware Connection
Connect them as the picture shows:

- 1. Connect the self-lock switch to the P0 port of the breadboard adapter.
  2. Connect the LED to P2 port of the breadboard through 100Ω resistor.

![](./images/k4dfMBY.jpg)

After connection, you will see:

![](./images/AuCiJU3.jpg)

### Software

Please open makecode.microbit.org(https://makecode.microbit.org/)  and write your code in the edit area.

![](./images/JHZUvh2.png)

### Add Package
- Not Required

### Program as the picture shows:

![](./images/bCNErri.png)

### Details for the code:
- 1.Set events monitor to P0 port and set it to high level.

![](./images/2jq655A.png)

- 2.Set the trigger for the event, when the self-lock switch is pressed down, the electric potential changes and the led lights on; while being pressed again, the electric potential changes again and the led lights off.

![](./images/TZcB7Jz.png)

### Reference
Links: [https://makecode.microbit.org/_Dhy5i9KVeLAK](https://makecode.microbit.org/_Dhy5i9KVeLAK)

You can also download the links directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Dhy5i9KVeLAK" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

## Result
---
Press down self-lock switch, LED lights on; press again, LED lights off. 

![](./images/sCMwXXf.gif)


## Exploration
---
Usually stair light uses double-throw switch to realize this function. We can turn on the light upstairs and turn off it downstairs. Vice versa. Suppose if we want to use 2 self-lock switch to realize stair light function, then how to design circuit and program? 

## FAQ
---



