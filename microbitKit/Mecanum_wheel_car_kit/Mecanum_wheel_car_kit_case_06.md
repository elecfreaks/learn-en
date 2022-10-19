# Case 06: Automatic Obstacle Avoidance 

## Purpose
---

- Build a Wonder Rugged Kit that can avoid obstacles.

## Products Link

[Wonder Rugged Car Kit](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-wonder-rugged-car-kit-without-micro-bit-board)
[Sonar:bit](https://shop.elecfreaks.com/search?type=product&q=Sonar%3Abit)

## Background Knowledge

------

## Software

------

[MicroSoft makecode](https://makecode.microbit.org/#)

## Program

------

### Step 1

Click "Advanced" in the drawer of MakeCode to see more choices. 

![](./images/Mecanum_wheel_car_kit_case_01_01.png)

For programming the Wonder Rugged Kit, we need to add a package. Click "Extensions" at the bottom of the drawer and then search "Wukong" in the dialogue box to download it. 

![](./images/Mecanum_wheel_car_kit_case_01_02.png)

For programming the ultrasonic sound sensor, we need to add a package. Click "Extensions" at the bottom of the drawer and then search "github.com/elecfreaks/pxt-sonarbit" in the dialogue box to download it. 

![](./images/Mecanum_wheel_car_kit_case_03_04.png)



***Note:*** If you get a warning indicating some packages will be removed because of incompatibility issues, you can follow the prompts or create a new project in the menu.

### Step 2

Click `Wukong` to choose `mecanum ` block.



![](./images/Mecanum_wheel_car_kit_case_01_03.png)


### Step 3

Drag `mecanum` into `on start`  block and set the connection for servos accordingly.



![](./images/Mecanum_wheel_car_kit_case_06_05.png)


### Step 4

Set the car to move forward and judge the distance between the obstacle and the car, if the distance is below 25cm, the car goes back with 500ms and turns left with 500ms.  

![](./images/Mecanum_wheel_car_kit_case_06_06.png)


### Program

Links: [https://makecode.microbit.org/_HD5CK8LmPWhH](https://makecode.microbit.org/_HD5CK8LmPWhH)

You can also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_HD5CK8LmPWhH]" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Result

The car moves forward after starting, if detecting any obstacles, it goes back and turns left to avoid the obstacle and then keeps going. 

## Exploration

------

## FAQ

------

## Relevant Files

---
