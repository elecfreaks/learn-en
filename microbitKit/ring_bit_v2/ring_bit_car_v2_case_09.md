# case 09 Remote Control by an accelerometer 

## Our Goal
---
- Use another an accelerometer of the micro:bit to remote control the car.

## Requiered Materials
---
- 1 x Ring:bit Car
- 2 x micro:bit

## Background 
---
### What is wireless ###

- Wireless technology sends message by radio wave because changes of electricity will generate waves. We can use this to load the message to the wave. Variation of electromagnetic field will generate the electricity when the electromagnetic is arrving the receiver. Then, to extract the message from wave by demodulation to send the message.

### What is an accelerometer ###

- The accelerometer is a kind of sensor to measure the accelerated speed. It has included mass block, damper, elastic component, sensitive element and optimal tuning circuit. The sensor is measuring the inertia force and getting the acceleration magnitude by newton's second law  during its accelerating. According to the difference of sensitive element, the common used accelerometer has included capacitance, strain, piezoresistive and piezoelectric.

 *The new version accelerometer chip of micro:bit is different from the old version. The new version has combined the electronic compass and the accelerometer. No change for usage.*

 ![](./images/2n6TbVZ.png)  ![](./images/F0frwo6.jpg)

## Hardware Connect
---
- Connect the left wheel servo to P1 of the Ring:bit expansion board and the right wheel servo to P2.
![](./images/jBVHea8.png)

## Software
---
[makecode](https://makecode.microbit.org/#)Online block coding[https://makecode.microbit.org/#](https://makecode.microbit.org/#)

## Coding
---
### Step 1
- Click on "Advanced" in the MakeCode Drawer to see more code sections.

![](./images/2qCyzQ7.png)

- Search for “ringbitcar” and click on the ring:bit car package to add it to your project. (As below picture)

![](./images/1Wq2Mov.jpg)

***Note：*** If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Project file menu.

### Step 2 ###

- It is difficult to calculate the control of the gyroscope, please refer more details by the link：Accelerometry

- If you don't want to type these code by yourself, you can directly download the whole program from the link below:

### Remote Control Coding
Program Link：[https://makecode.microbit.org/_AT4PoHKdVi6L](https://makecode.microbit.org/_AT4PoHKdVi6L)

If you don't want to type these code by yourself, you can directly download the whole program from the link below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_AT4PoHKdVi6L" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Ring:bit car Coding ###
Program Link：[https://makecode.microbit.org/_e5t6XPHoTiHy](https://makecode.microbit.org/_e5t6XPHoTiHy)

If you don't want to type these code by yourself, you can directly download the whole program from the link below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_e5t6XPHoTiHy" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


## Result
---
- The Ring:bit car will move as direction of the gyroscope and its speed will as the angle of inclination of the gyroscope.


## Think
---
- 

## Questions
---


## More Information   
---

