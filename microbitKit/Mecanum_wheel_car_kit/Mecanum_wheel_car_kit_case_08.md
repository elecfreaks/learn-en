# Case 08: Search for Light

## Purpose
---

- Build a Wonder Rugged Kit that can search for light.

## Products Link

[Wonder Rugged Car Kit](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-wonder-rugged-car-kit-without-micro-bit-board)

## Background Knowledge
---

## Software
---

[MicroSoft makecode](https://makecode.microbit.org/#)

## Program
---

### Step 1

Click "Advanced" in the drawer of MakeCode to see more choices. 

![](./images/Mecanum_wheel_car_kit_case_01_01.png)

For programming the Wonder Rugged Kit, we need to add a package. Click "Extensions" at the bottom of the drawer and then search "Wukong" in the dialogue box to download it. 

![](./images/Mecanum_wheel_car_kit_case_01_02.png)

***Note:*** If you get a warning indicating some packages will be removed because of incompatibility issues, you can follow the prompts or create a new project in the menu.

### Step 2

Click `Wukong` to choose `mecanum ` block.

![](./images/Mecanum_wheel_car_kit_case_01_03.png)

### Step 3

Drag `mecanum` into `on start`  block and set the connection for servos accordingly, then initialize the LEDs.



![](./images/Mecanum_wheel_car_kit_case_08_05.png)


### Step 4

Set variable `i` as the brightness level and judge the value of it. If the value of `i` is below 50, the car turns left; or it moves forward. 



![](./images/Mecanum_wheel_car_kit_case_08_06.png)


### Program 

Links: [https://makecode.microbit.org/_Kv3dfY02f52g](https://makecode.microbit.org/_Kv3dfY02f52g)

You can also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Kv3dfY02f52g]" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Result

The car spins itself if no light being detected, or it goes straight towards the light. 

## Exploration
---

If we want the farther away the car is from the light source, the faster it is; and the closer it is to the light source, the slower it is, how to programme? 

## FAQ
---

## Relevant Files
---
