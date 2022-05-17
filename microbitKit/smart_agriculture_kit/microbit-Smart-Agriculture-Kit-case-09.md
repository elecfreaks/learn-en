# Case 09: Crops Sunshade Device


##  Introduction
---

- Although the growth of plants depends on photosynthesis. However, the strong light may also cause physiological damage to plants. When the light is too strong, it is easy to cause leaf burn or sunburn, thus, we can make a crop sunshade device to protect the crops. 

##  Function
---
- Detect the light intensity through the light sensor on the micro:bit, if it's strong, program to drive the servo to lift the sunshade device. 

## Products Link
---
- 1 x [microbit Smart Agriculture Kit]()

## Picture
---
![](./images/microbit-Smart-Agriculture-Kit-case-01-02.png)

## Hardware Connection

---

Connect the servo to P1 on IoT:bit. 

![](./images/microbit-Smart-Agriculture-Kit-case-08-03.png)

## Software Programming 

---

Click "Advanced" in the MakeCode to see more choices.

![](./images/microbit-Smart-Agriculture-Kit-case-01-04.png)

For programming, we need to add a package: click "Extensions" at the bottom of the MakeCode drawer and search with "servo" in the dialogue box to download it. 

![](./images/microbit-Smart-Agriculture-Kit-case-01-06.png)

***Notice:*** If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu. 

## Program

---

In forever block, judge if the light intensity is over 200. 

![](./images/microbit-Smart-Agriculture-Kit-case-09-07.png)

If yes, program the servo to drive to 90°; or set the servo to drive to 0°.

![](./images/microbit-Smart-Agriculture-Kit-case-09-08.png)



Link: [https://makecode.microbit.org/_hctVTMDirM8x](https://makecode.microbit.org/_hctVTMDirM8x)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_hctVTMDirM8x" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result
---
- If the light intensity is too strong, the sunshade device will be lifted automatically to protect the crops. 



