# Case 06: Insect-catching Device


##  Introduction
---

- In agricultural planting, insect pests affect the yield and the quality of crops. Pests are active at night, gnawing, laying eggs and breeding crops are also carried out at night. Thus, we can make use of the phototaxis of pests to make an automatic insect-catching device that attracts and catches them.

##  Function
---
- Attract the pests through the LED and drive the servo to catch them.

## Products Link
---
- 1 x [microbit Smart Agriculture Kit](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-smart-agriculture-kit-without-micro-bit-board?_pos=2&_sid=2c86b7764&_ss=r)

## Picture
---
![](./images/microbit-Smart-Agriculture-Kit-case-01-02.png)

## Hardware Connection
---

Connect the Rainbow LED to P1 and the servo to P2 on IoT:bit. 

![](./images/microbit-Smart-Agriculture-Kit-case-06-03.png)

## Software Programming 

---

Click "Advanced" in the MakeCode to see more choices.

![](./images/microbit-Smart-Agriculture-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "neopixel" in the dialogue box to download it. 

![](./images/microbit-Smart-Agriculture-Kit-case-03-06.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "servo" in the dialogue box to download it. 

![](./images/microbit-Smart-Agriculture-Kit-case-01-06.png)

***Notice:*** If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

## Program

---

Drag the on start block from the drawer, initialize the strip connecting to P1 with 1 led, program to show white color. 

![](./images/microbit-Smart-Agriculture-Kit-case-06-07.png)

Drag the forever block from the drawer, set  the servo connecting to P2 to drive to 0°, pause for 1 sec and set the servo to drive to 180° and pause another 5 sec. 


![](./images/microbit-Smart-Agriculture-Kit-case-06-08.png)

Link: [https://makecode.microbit.org/_ae72379ieU5W](https://makecode.microbit.org/_ae72379ieU5W)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_ae72379ieU5W" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result 
---
- After powering on, the LED lights on in white and the servo rotates every 5 seconds. 



