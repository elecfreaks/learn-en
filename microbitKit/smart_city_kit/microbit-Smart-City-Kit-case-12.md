# Case 12: The Burglar Alarm in Shops


##  Introduction
---

- After installing the bulglar alarm device in shops, program to send alarms if someone breaks into the shops. 

##  Function

- Detect the magnet from the magnetic(compass) function on the micro:bit,  if the magnet goes far from the micro:bit, program to send alarms and light on the LED. 

## Products Link
---
- 1 x [microbit Smart City Kit]()
Note: A piece of magnet requires in this project.

## Picture
---
![](./images/microbit-Smart-City-Kit-case-01-02.png)

## Hardware Connection
---

Connect the red led to P1 port on IoT:bit. 

![](./images/microbit-Smart-City-Kit-case-12-03.png)

## Software Program

---

Click "Advanced" in the MakeCode drawer to see more choices. 

![](./images/microbit-Smart-City-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "iot-environment-kit" in the dialogue box to download it. 

![](./images/microbit-Smart-City-Kit-case-01-05.png)



Notice: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

## Program

---

Detect the magnetic intensity in the current field, if the returned value is below the threhold, program to send alarms and flash on the led. 

![](./images/microbit-Smart-City-Kit-case-12-07.png)

Link: [https://makecode.microbit.org/_0fiexRbyoKpE](https://makecode.microbit.org/_0fiexRbyoKpE)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_0fiexRbyoKpE" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result
---
- If someone breaks into the shop, the device sends alarms and the led keeps flashing. 



