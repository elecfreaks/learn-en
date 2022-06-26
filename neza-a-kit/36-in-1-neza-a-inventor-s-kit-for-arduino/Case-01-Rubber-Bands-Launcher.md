# Case 01: Rubber Bands Launcher
## Purpose
---
Make a rubber bands launcher through  [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html).
![](./images/neza-a-case-01-01.png)

## Purchase Link
---
  [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html)

## Materials Required
---
![](./images/neza-a-case-01-02.png)
## Assembly steps 
---
![](./images/neza-a-step-01-01.png)
![](./images/neza-a-step-01-02.png)
![](./images/neza-a-step-01-03.png)
![](./images/neza-a-step-01-04.png)
![](./images/neza-a-step-01-05.png)
![](./images/neza-a-step-01-06.png)
![](./images/neza-a-step-01-07.png)
![](./images/neza-a-step-01-08.png)
![](./images/neza-a-step-01-09.png)
![](./images/neza-a-step-01-10.png)
![](./images/neza-a-step-01-11.png)
![](./images/neza-a-step-01-12.png)
![](./images/neza-a-step-01-13.png)
![](./images/neza-a-step-01-14.png)
![](./images/neza-a-step-01-15.png)
![](./images/neza-a-step-01-16.png)
![](./images/neza-a-step-01-17.png)
![](./images/neza-a-step-01-18.png)
![](./images/neza-a-step-01-19.png)
![](./images/neza-a-step-01-20.png)
![](./images/neza-a-step-01-21.png)
![](./images/neza-a-step-01-22.png)
![](./images/neza-a-step-01-23.png)
![](./images/neza-a-step-01-24.png)
![](./images/neza-a-step-01-25.png)
![](./images/neza-a-step-01-26.png)
![](./images/neza-a-step-01-27.png)
![](./images/neza-a-step-01-28.png)
![](./images/neza-a-step-01-29.png)
![](./images/neza-a-step-01-30.png)
![](./images/neza-a-step-01-31.png)
![](./images/neza-a-step-01-32.png)
![](./images/neza-a-step-01-33.png)
![](./images/neza-a-step-01-34.png)

Wrap the rubber bands with the device:
![](./images/neza-a-case-01-03.gif)

## Hardware Connection
---
Connect the [two buttons](https://www.elecfreaks.com/planetx-button.html) to J1 port and the [Servo](https://www.elecfreaks.com/geekservo-2kg-360-degrees-compatible-with-lego.html) to S1 port on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 
![](./images/neza-a-case-01-04.png)

## Programming
---
### Prepare the programming
Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html)
Import the libraries and the subsidiary libraries of [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html) and then import the libraries of the [two buttons](https://www.elecfreaks.com/planetx-button.html):  [PlanetXButton-main.zip](https://github.com/elecfreaks/PlanetXButton/archive/refs/heads/main.zip)
Download and import the self-defined library connections for [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html): [RJPins-main.zip](https://github.com/elecfreaks/RJPins/archive/refs/heads/main.zip)

### Sample Code: 
```python
#include <PlanetXButton.h>
#include <NezhaA.h>
#include <RJPins.h>

PlanetXButton buttonJ1(J1);    //Create an instance of PlanetXButton category
NezhaA nezhaA;    //Create an instance of NezhaA category

void setup() {
  nezhaA.begin();    //Initiliaze the buzzer, motor, servo and light
}

void loop() {
  if (buttonJ1.isPressed(C)) {    //While button C is pressed
    nezhaA.setServoAngle(S1, 190);    //Set the angle of the servo as 200 degrees at S1 port. 
  }
  if (buttonJ1.isPressed(D)) {
    nezhaA.setServoAngle(S1, 270);    
  }
}
```

### Result
Control the rubber band through this rubber band launcher. 
![](./images/neza-a-case-01-05.gif)

***Note*** The angle of the servo that controls the launch needs to be adjusted according to the number of rubber bands. Using too many rubber bands will cause excessive tension and damage the servos. It is recommended that no more than three rubber bands be used for launching.

