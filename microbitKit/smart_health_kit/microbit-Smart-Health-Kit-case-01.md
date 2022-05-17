# Case 01: Touch-free Hands Washing Device


##  Introduction
---

- Maintaining clean and hygienic hands can prevent diseases from entering the mouth, thereby reducing the risk of intestinal infectious diseases such as diarrhea and respiratory infectious diseases such as pneumonia. After washing our hands, we need to close the water valve, which will cause pollution to our hands, thus, we can make a touch-free hand washing device.

## Function
---

- Detect if there is anyone approaching with the PIR sensor, if yes, program to open the water valve. 

## Products Link
---
- 1 x [micro:bit Smart Health Kit]()

## Picture
---
![](./images/microbit-Smart-Health-Kit-case-01-02.png)

## Hardware Connection
---

Connect the PIR sensor to P1 and the servo to P2 on sensor:bit. 

![](./images/microbit-Smart-Health-Kit-case-01-03.png)

## Software Programming 
---

Click "Advanced" in the MakeCode to see more choices.

![](./images/microbit-Smart-Health-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "smarthome" in the dialogue box to download it. 

![](./images/microbit-Smart-Health-Kit-case-01-05.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "servo" in the dialogue box to download it. 

![](./images/microbit-Smart-Health-Kit-case-01-06.png)

***Notice:*** If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

## Program 
---
Judge the detected motion of  variable "IR", if yes, set to show "√" and the servo to drive to 0° to open the water valve; or set to show "x" and to drive to 180° to close the water valve. 

![](./images/microbit-Smart-Health-Kit-case-01-07.png)

Link: [https://makecode.microbit.org/_KuhhtHVds1EH](https://makecode.microbit.org/_KuhhtHVds1EH)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_KuhhtHVds1EH" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result
---
- If the PIR sensor detects someone, program to open the water valve; or program to close it. 



