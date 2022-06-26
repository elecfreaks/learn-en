# Case 03: A Small Forklift

## Purpose
---
Make a small forklift with [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html).

![](./images/neza-a-case-03-01.png)

## Purchse
---
 [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html)

## Materials Required
---
![](./images/neza-a-case-03-02.png)

## Assembly Steps
---
![](./images/neza-a-step-03-01.png)
![](./images/neza-a-step-03-02.png)
![](./images/neza-a-step-03-03.png)
![](./images/neza-a-step-03-04.png)
![](./images/neza-a-step-03-05.png)
![](./images/neza-a-step-03-06.png)
![](./images/neza-a-step-03-07.png)
![](./images/neza-a-step-03-08.png)
![](./images/neza-a-step-03-09.png)
![](./images/neza-a-step-03-10.png)
![](./images/neza-a-step-03-11.png)
![](./images/neza-a-step-03-12.png)
![](./images/neza-a-step-03-13.png)
![](./images/neza-a-step-03-14.png)
![](./images/neza-a-step-03-15.png)
![](./images/neza-a-step-03-16.png)
![](./images/neza-a-step-03-17.png)
![](./images/neza-a-step-03-18.png)
![](./images/neza-a-step-03-19.png)
![](./images/neza-a-step-03-20.png)
![](./images/neza-a-step-03-21.png)
![](./images/neza-a-step-03-22.png)
![](./images/neza-a-step-03-23.png)
![](./images/neza-a-step-03-24.png)
![](./images/neza-a-step-03-25.png)
![](./images/neza-a-step-03-26.png)
![](./images/neza-a-step-03-27.png)
![](./images/neza-a-step-03-28.png)
![](./images/neza-a-step-03-29.png)
![](./images/neza-a-step-03-30.png)
![](./images/neza-a-step-03-31.png)
![](./images/neza-a-step-03-32.png)
![](./images/neza-a-step-03-33.png)
![](./images/neza-a-step-03-34.png)
![](./images/neza-a-step-03-35.png)
![](./images/neza-a-step-03-36.png)
![](./images/neza-a-step-03-37.png)
![](./images/neza-a-step-03-38.png)
![](./images/neza-a-step-03-39.png)
![](./images/neza-a-step-03-40.png)
![](./images/neza-a-step-03-41.png)
![](./images/neza-a-step-03-42.png)
![](./images/neza-a-step-03-43.png)
![](./images/neza-a-step-03-44.png)
![](./images/neza-a-step-03-45.png)
![](./images/neza-a-step-03-46.png)
![](./images/neza-a-step-03-47.png)
![](./images/neza-a-step-03-48.png)
![](./images/neza-a-step-03-49.png)
![](./images/neza-a-step-03-50.png)

## Hardware Connections
---
Connect two [motors](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 and M2,  the [two buttons](https://www.elecfreaks.com/planetx-button.html) to J1 port on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 
![](./images/neza-a-case-03-03.png)

## Programming
---
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html)

Import the libraries and the subsidiary libraries of [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html) and then import the libraries of the [two buttons](https://www.elecfreaks.com/planetx-button.html):  [PlanetXButton-main.zip](https://github.com/elecfreaks/PlanetXButton/archive/refs/heads/main.zip)
Download and import the self-defined library connections for [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html): [RJPins-main.zip](https://github.com/elecfreaks/RJPins/archive/refs/heads/main.zip)

### Sample Projects:

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
    nezhaA.setMotorSpeed(M1, 50);   // Set the speed of the motor connecting to M1 at 50%
    delay((2) * 1000);    //Pause 2000ms
    nezhaA.brakeMotor(M1);    //Stop the motor connecting to M1
    nezhaA.setMotorSpeed(M2, 100);   //Set the speed of the motor connecting to M2 at 100%
    delay((1) * 1000);
    nezhaA.brakeMotor(M2);    //设Stop the motor connecting to M2
  }
  if (buttonJ1.isPressed(D)) {    //While button D is pressed
    nezhaA.setMotorSpeed(M1, -50);
    delay((2) * 1000);
    nezhaA.brakeMotor(M1);
    nezhaA.setMotorSpeed(M2, -100);
    delay((1) * 1000);
    nezhaA.brakeMotor(M2);
  }
}
```
### Result
After powering on, press button C and the car drives forward for 2 seconds and the raise its folklift; press button D and the car reverses for 2 seconds, then it puts the folklift down. 

