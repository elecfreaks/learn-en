# Lesson 02 Button  
 
 ![](./images/SVbSfPB.jpg)

## Introduction:

In our previous experiment , we have learned how to use Micro:bit to control 2 LEDs and make them twinkle alternatively. This time we are going to use a button to control LED flash. That means when we press down the button,the 2 LEDs flash in turns; when release the button, the LEDs stop flashing.

## Components List:

### Hardware:
- 1 x Micro:bit Board
- 1 x Micro-B USB Cable
- 1 x Microbit Breadboard Adapter
- 1 x Transparent Breadboard - 83 * 55 mm
- 2 x LED
- 2 x 100 Ohm Resistors
- 1 x Momentary Pushbutton Switch
- n x Breadborad jumper wire 65pcs pack

***Tips: If you want to buy all components above, you may need Elecfreaks Micro:bit  [Starter Kit](https://www.elecfreaks.com/micro-bit-starter-kit.html)  .***

![](./images/W4tseua.jpg)

## Major Components Introduction

### Momentary Pushbutton Switch

This is a common component for controlling electronic devices. It is mostly used to connect or cut off the control circuit, it can achieve the control for motors or other electronic equipments.

 Momentary Pushbutton Switch usually stays on. When it is pressed down, the circuit is connected; when it is released, it will bounce back to the status of disconnection.

![](./images/IO2KzaW.jpg)

Momentary Pushbutton Switch has 4 pins which can be divided into 2 groups: pin 1 short connects pin 2, pin 3 short connects pin 4.

![](./images/OgWZfBQ.jpg)


## Experimental Procedure

### Hardware Connection

Connect your components according to the picture below: 

- 1.Connect the shorter leg with the GND.
- 2.Connector the longer leg with the P0 and P1 ports through the Resistor.
- 3.Connect the Momentary Pushbutton to P2 port.

![](./images/qXKoSN4.jpg) 

You would see as below after you finish the connection: 

![](./images/uGLigLh.jpg)

### Software Programming

Click to open [Microsoft Makecode](https://makecode.microbit.org/), write the following code in the editor.

![](./images/JHZUvh2.png)

### Program as the picture shows:

![](./images/SHgMhjZ.png)

### Details for the code:
- 1.Set pin P2 to the high potential in the bricks of "on start".

![](./images/pS67VCj.png)

- 2.Read the status from P2 to check if the button is pressed, if yes, digital write signal 0 to P0 port to turn off the LED; digital write signal 1 to P1 port to turn on the LED,  then set the pause in 500ms; digital write signal 1 to P0 port to turn on the LED; digital write signal 0 to P1 port to turn off the LED,  then set the pause in 500ms.

![](./images/mpKfkU4.png)

### Reference
Links: [https://makecode.microbit.org/_T585WeYwVWtv](https://makecode.microbit.org/_T585WeYwVWtv)

You can also download the links directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_T585WeYwVWtv" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


## Result

When the button is pressed, you can see the  2 LEDs flashing alternatively; When the button is released, they would stop flashing. If not, you need to go back and check your operations.

![](./images/7w5yp6z.gif)


## Exploration

If we want to light  on the red LED when press the button and light on the green LED when release the button,  how can we program? 

## FAQ

