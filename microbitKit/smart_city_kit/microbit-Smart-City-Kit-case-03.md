# Case 03: Smart Trash Can

##  Introduction
---

Most of the trash cans sit on the roadside are designed by throwing in the trash from the side part without lids, the bad smell are easily to get especially in hot summer days, and there are some cans with lids but require us to open it by hands, which may easily get virus and dirt attached to our body. Therefore, we could design a smart trash can to open the lids by itself while there are people appraching and close when they are leaving. 

##  Function

---

Detect if there are humans approaching with the sonar:bit, program to open the lid automatically when people come and to close when they leave. 

## Products Link
---
- 1 x [microbit Smart City Kit]()

## Picture
---
![](./images/microbit-Smart-City-Kit-case-01-02.png)

## Hardware Connection 
---

Connect the sonar:bit to P1,  the servo to P2 on IoT:bit. 

## Software Programming 

---

Click "Advanced" in the MakeCode to see more choices.

![](./images/microbit-Smart-City-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "iot-environment-kit" in the dialogue box to download it. 

![](./images/microbit-Smart-City-Kit-case-01-05.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "servo" in the dialogue box to download it. 

![](./images/microbit-Smart-City-Kit-case-01-06.png)

## Program 

---

Save the returned ultrasonic distance value as the variable “ultrasonic_distance”. 

![](./images/microbit-Smart-City-Kit-case-03-07.png)

Detect if there are people near the trash cans through the sonar:bit(note the detection range is 4~400cm), if the object is not in this scope, the returned value would be 0, therefore, here we need to define both of the minum and maxium value.  

![](./images/microbit-Smart-City-Kit-case-03-08.png)

If the varible value is in the scope, it means there are people approching the cans, program to turn on the servo and open the lid, or it closes. 

![](./images/microbit-Smart-City-Kit-case-03-09.png)

Link: [https://makecode.microbit.org/_LP22ogi0t1KJ](https://makecode.microbit.org/_LP22ogi0t1KJ)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_LP22ogi0t1KJ" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result
---
- If there are people approching the cans, the lid would be opened automatically or it closes. 



