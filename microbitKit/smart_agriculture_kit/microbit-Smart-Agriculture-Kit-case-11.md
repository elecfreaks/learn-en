# Case 11: Feed at Fixed Time


##  Introduction
---

- Feeding animals in manual is not convenient, we can make a device that could feed them at fixed time. 

##  Function
---
- Make the timing with RTC module and program to drive the servo for feeding at the fixed time. 

## Products Link
---
- 1 x [microbit Smart Agriculture Kit]()

## Picture
---
![](./images/microbit-Smart-Agriculture-Kit-case-01-02.png)

## Hardware Connection
---

Connect the servo to P1, and the OLED to IIC on IoT:bit. 

![](./images/microbit-Smart-Agriculture-Kit-case-11-03.png)

## Software Programming 

---

Click "Advanced" in the MakeCode to see more choices.

![](./images/microbit-Smart-Agriculture-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "iot-environment-kit" in the dialogue box to download it. 

![](./images/microbit-Smart-Agriculture-Kit-case-01-05.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "neopixel" in the dialogue box to download it. 

![](./images/microbit-Smart-Agriculture-Kit-case-01-06.png)

Notice: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

## Program

---

Initialize the OLED display as 128×64m and the time settings of RTC module, set the sevo to drive to 0°.

![](./images/microbit-Smart-Agriculture-Kit-case-11-07.png)

Display the current seconds on OLED screen. 

![](./images/microbit-Smart-Agriculture-Kit-case-11-08.png)

If the second is 1, set the servo to drive to 90°, pause 5000ms and then set the servo to drive to 0°. 

![](./images/microbit-Smart-Agriculture-Kit-case-11-09.png)

Link: [https://makecode.microbit.org/_RE7cgtJCJMFP](https://makecode.microbit.org/_RE7cgtJCJMFP)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_RE7cgtJCJMFP" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result
---
- The device makes the feeding every 1 minute. 
