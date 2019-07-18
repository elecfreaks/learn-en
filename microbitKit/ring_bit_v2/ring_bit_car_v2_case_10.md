# Case 10 Smart Crashproof Car

## Purpose
---
- Make a smart crashproof car with a Sonar:bit. 

## Materials
---
- 1 x Ring:bit Car kit
- 1 x micro:bit 
- 1 x Sonar:bit


## Hardware Connection
---
- Connect the left servo to P1, right servo to P2 and Sonar:bit to P0 of the Ring:bit.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/case_10_01.png)

## Software Programming
---
[Microsoft makecode online coding https://makecode.microbit.org/#](https://makecode.microbit.org/#)

## Software
---
### Step 1
- Click "Advanced" in the drawer of MakeCode to see more choices.

![](./images/2qCyzQ7.png)

- We need to add a package for programming the kit. Click "Extensions" in the drawer and search “ringbit" in the dialogue box to download it. 

![](./images/1Wq2Mov.jpg)

- We also need to add a package for programming the Sonar:bit. Click "Extensions" in the drawer and search “`https://github.com/elecfreaks/pxt-sonarbit`" in the dialogue box to download it. 

Note: if you are informed that it will be deleted due to incompatibility of the codebase, you can go on with the tips or create a new project in the menu.

### Step 2

- Drag the pins selection bricks for servos in the `On start` brick, the pins numbers are set according to the actual connection port.
- Move forward at full speed.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/case_10_02.png)

### Step 3

- Set variate `sonar` in the `forever` brick and read the detected value from the Sonar:bit to it. 
- Drag the `if` brick and judge if the value given by `sonar` is below 10 and not equal to 0. 
- If yes, set the speed of right wheel to 100 and the left to 0 to turn left for obstacle avoidance. 
- If not, move forward at full speed.

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/ring_bit_v2/images/case_10_03.png)

### Reference

Links: [https://makecode.microbit.org/_RMU80R85iVvv](https://makecode.microbit.org/_RMU80R85iVvv)

You can also download it below: 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_RMU80R85iVvv" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---



## Result 
---
- The Ring:bit car turns left automatically when detecting any obstacle 10cm in front of it.


## Exploration
---
- Question: Why we need to judge if the value is not 0 ?
- Answer: The detection value is also 0 if beyond the detection scope of Sonar:bit. 

## FAQ
---

