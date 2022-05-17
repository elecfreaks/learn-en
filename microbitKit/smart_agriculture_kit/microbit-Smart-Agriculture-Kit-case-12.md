# Case 12: Birds Anti-Collision Device


##  Introduction
---

- Bird hitting buildings or bird hitting glass refers to the fact that birds cannot recognize the existence of glass due to the transparent and reflective properties of the glass, and thus collide with buildings, especially glass windows, causing the birds to be injured or killed. Bird hitting buildings is one of the most serious threats to birds. One of the preventive measures is to turn off unnecessary lights or draw curtains at night. Because at night, the decorative light near the glass can disorient the migrating birds, causing them to collide with skyscrapers, office buildings or other glass decorated with lights. So we can design a device that automatically draws the curtains to reduce light interference.

##  Function
---
- Detect the light intensity with the light sensor on the micro:bit, if the light intensity is below the threshold, program to drive the servo to draw the curtains. 

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

In forever block, judge if the current light level is below 20.

![](./images/microbit-Smart-Agriculture-Kit-case-12-07.png)

If yes, program to set the servo connecting to P1 to drive to 180°; or to drive to 0°.

![](./images/microbit-Smart-Agriculture-Kit-case-12-08.png)


Link: [https://makecode.microbit.org/_dHgWHFfYvgTR](https://makecode.microbit.org/_dHgWHFfYvgTR)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_dHgWHFfYvgTR" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  


## Result 
---
- If the light level is below the threshold, the servo drives to draw the curtains. 



