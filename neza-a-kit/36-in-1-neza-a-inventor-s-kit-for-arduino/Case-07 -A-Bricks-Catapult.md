# Case 07: A Bricks Catapult

## Purpose
---
Make a bricks catapult with [NezhaA Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-arduino-36-in-1-nezha-a-inventors-kit?_pos=2&_sid=e1dfa3343&_ss=r).
![](./images/neza-a-case-07-01.png)

## Purchse
---
 [NezhaA Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-arduino-36-in-1-nezha-a-inventors-kit?_pos=2&_sid=e1dfa3343&_ss=r)

## Materials Required
---
![](./images/neza-a-case-07-02.png)

## Assembly Steps
---
![](./images/neza-a-step-07-01.png)
![](./images/neza-a-step-07-02.png)
![](./images/neza-a-step-07-03.png)
![](./images/neza-a-step-07-04.png)
![](./images/neza-a-step-07-05.png)
![](./images/neza-a-step-07-06.png)
![](./images/neza-a-step-07-07.png)
![](./images/neza-a-step-07-08.png)
![](./images/neza-a-step-07-09.png)
![](./images/neza-a-step-07-10.png)
![](./images/neza-a-step-07-11.png)
![](./images/neza-a-step-07-12.png)
![](./images/neza-a-step-07-13.png)
![](./images/neza-a-step-07-14.png)
![](./images/neza-a-step-07-15.png)
![](./images/neza-a-step-07-16.png)
![](./images/neza-a-step-07-17.png)
![](./images/neza-a-step-07-18.png)
![](./images/neza-a-step-07-19.png)
![](./images/neza-a-step-07-20.png)
![](./images/neza-a-step-07-21.png)
![](./images/neza-a-step-07-22.png)
![](./images/neza-a-step-07-23.png)
![](./images/neza-a-step-07-24.png)
![](./images/neza-a-step-07-25.png)
![](./images/neza-a-step-07-26.png)
![](./images/neza-a-step-07-27.png)
![](./images/neza-a-step-07-28.png)
![](./images/neza-a-step-07-29.png)
![](./images/neza-a-step-07-30.png)
![](./images/neza-a-step-07-31.png)
![](./images/neza-a-step-07-32.png)
![](./images/neza-a-step-07-33.png)
![](./images/neza-a-step-07-34.png)

## Hardware Connections
---
Connect the [motor](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 port and the[two buttons](https://www.elecfreaks.com/planetx-button.html) to J1 port on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 

![](./images/neza-a-case-07-03.png)

## Programming
---
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html)
Import the libraries and the subsidiary libraries of [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html) and then import the libraries of the [two buttons](https://www.elecfreaks.com/planetx-button.html):  [PlanetXButton-main.zip](https://github.com/elecfreaks/PlanetXButton/archive/refs/heads/main.zip)
Download and import the self-defined library connections for [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html): [RJPins-main.zip](https://github.com/elecfreaks/RJPins/archive/refs/heads/main.zip)

### Sample Code: 

```
// Language ArduinoC
#include <RJPins.h>
#include <NezhaA.h>
#include <PlanetXButton.h>

PlanetXButton buttonJ1(J1);    //Create an instance of PlanetXButton category
NezhaA nezhaA;    //Create an instance of NezhaA category

void setup() {
  nezhaA.begin();    //Initiliaze the buzzer, motor, servo and light
}

void loop() {
  if (buttonJ1.isPressed(C)) {    //While button C is pressed
    nezhaA.setMotorSpeed(M1, 30);   //Set the speed of the motor connecting to M1 at 50%
    delay((0.5) * 1000);    //Pause 500ms
    nezhaA.brakeMotor(M1);    //Stop the motor connecting to M1
  }
  if (buttonJ1.isPressed(D)) {    //While button D is pressed
    nezhaA.setMotorSpeed(M1, -100);
    delay((0.5) * 1000);
    nezhaA.brakeMotor(M1);
  }
}
```
### Result
After powering on, press button C to lift the pole, then press button D and the bricks would be flapped out by the pole. 

