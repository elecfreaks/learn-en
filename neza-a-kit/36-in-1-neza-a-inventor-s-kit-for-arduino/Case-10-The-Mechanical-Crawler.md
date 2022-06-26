# Case 10: The Mechanical Crawler

## Purpose
---
Make a mechanical crawler with [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html).

![](./images/neza-a-case-10-01.png)

## Purchse
---
 [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html)

## Materials Required
---
![](./images/neza-a-case-10-02.png)

## Assembly Steps
---
![](./images/neza-a-step-10-01.png)
![](./images/neza-a-step-10-02.png)
![](./images/neza-a-step-10-03.png)
![](./images/neza-a-step-10-04.png)
![](./images/neza-a-step-10-05.png)
![](./images/neza-a-step-10-06.png)
![](./images/neza-a-step-10-07.png)
![](./images/neza-a-step-10-08.png)
![](./images/neza-a-step-10-09.png)
![](./images/neza-a-step-10-10.png)
![](./images/neza-a-step-10-11.png)
![](./images/neza-a-step-10-12.png)
![](./images/neza-a-step-10-13.png)
![](./images/neza-a-step-10-14.png)
![](./images/neza-a-step-10-15.png)
![](./images/neza-a-step-10-16.png)
![](./images/neza-a-step-10-17.png)
![](./images/neza-a-step-10-18.png)
![](./images/neza-a-step-10-19.png)
![](./images/neza-a-step-10-20.png)
![](./images/neza-a-step-10-21.png)
![](./images/neza-a-step-10-22.png)
![](./images/neza-a-step-10-23.png)
![](./images/neza-a-step-10-24.png)
![](./images/neza-a-step-10-25.png)
![](./images/neza-a-step-10-26.png)
![](./images/neza-a-step-10-27.png)
![](./images/neza-a-step-10-28.png)

## Hardware Connections
---
Connect the [motor](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 port on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 

![](./images/neza-a-case-09-03.png)

## Programming
---
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html).

### Sample Code: 

```
// Language ArduinoC
#include <NezhaA.h>

NezhaA nezhaA;    //Create an instance of Nezha category

void setup() {
  nezhaA.begin();    //Initiliaze the buzzer, motor, servo and light
  nezhaA.setMotorSpeed(M1, 100);    //Set the speed of the motor connecting to M1 at 100%
}

void loop() {

}

```
### Result
After powering on, it crawls forward. 
