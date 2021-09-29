# Case 05: Water Temperature Detection 


##  Introduction
---

- Fishes are poikilotherm whose body temperature changes as the ambient water temperature changes, thus, the water temperature plays a vital role in the growth of fishes. 

##  Function
---
- Dectect the water temperature with the DS18B20 sensor and display them on OLED screen. 

## Products Link
---
- 1 x [microbit Smart Agriculture Kit]()

## Picture
---
![](./images/microbit-Smart-Agriculture-Kit-case-01-02.png)

## Hardware Connection
---

Connect DS18B20 to P1 and the OLED to IIC on IoT:bit. 

![](./images/microbit-Smart-Agriculture-Kit-case-05-03.png)

## Software Programming 

---

Click "Advanced" in the MakeCode to see more choices.

![](./images/microbit-Smart-Agriculture-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "iot-environment-kit" in the dialogue box to download it. 

![](./images/microbit-Smart-Agriculture-Kit-case-01-05.png)

Notice: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

## Program

---

Initialize the OLED screen as 128×64.

![](./images/microbit-Smart-Agriculture-Kit-case-05-07.png)

Set  DS18B20 sensor to connect to P1 and save the returned value as variable "Temp".

![](./images/microbit-Smart-Agriculture-Kit-case-05-08.png)

Clear the OLED screen and display the water temperature. 

![](./images/microbit-Smart-Agriculture-Kit-case-05-09.png)

Link: [https://makecode.microbit.org/_Jx2d4JgU6iWj](https://makecode.microbit.org/_Jx2d4JgU6iWj)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_Jx2d4JgU6iWj" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result
---
- The OLED displays the water temperature and refreshes every 5 seconds. 



