# Case 05:  A Line-follwing Car

## Purpose
---
Make a line-following car with [NezhaA Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-arduino-36-in-1-nezha-a-inventors-kit?_pos=2&_sid=e1dfa3343&_ss=r).

![](./images/neza-a-case-05-01.png)

## Purchse
---
 [NezhaA Inventor's Kit](https://shop.elecfreaks.com/products/elecfreaks-arduino-36-in-1-nezha-a-inventors-kit?_pos=2&_sid=e1dfa3343&_ss=r)

## Materials Required
---
![](./images/neza-a-case-05-02.png)

## Assembly Steps
---
![](./images/neza-a-step-05-01.png)
![](./images/neza-a-step-05-02.png)
![](./images/neza-a-step-05-03.png)
![](./images/neza-a-step-05-04.png)
![](./images/neza-a-step-05-05.png)
![](./images/neza-a-step-05-06.png)
![](./images/neza-a-step-05-07.png)
![](./images/neza-a-step-05-08.png)
![](./images/neza-a-step-05-09.png)
![](./images/neza-a-step-05-10.png)
![](./images/neza-a-step-05-11.png)
![](./images/neza-a-step-05-12.png)
![](./images/neza-a-step-05-13.png)
![](./images/neza-a-step-05-14.png)
![](./images/neza-a-step-05-15.png)
![](./images/neza-a-step-05-16.png)
![](./images/neza-a-step-05-17.png)
![](./images/neza-a-step-05-18.png)
![](./images/neza-a-step-05-19.png)
![](./images/neza-a-step-05-20.png)
![](./images/neza-a-step-05-21.png)
![](./images/neza-a-step-05-22.png)
![](./images/neza-a-step-05-23.png)
![](./images/neza-a-step-05-24.png)
![](./images/neza-a-step-05-25.png)
![](./images/neza-a-step-05-26.png)
![](./images/neza-a-step-05-27.png)
![](./images/neza-a-step-05-28.png)
![](./images/neza-a-step-05-29.png)
![](./images/neza-a-step-05-30.png)
![](./images/neza-a-step-05-31.png)
![](./images/neza-a-step-05-32.png)
![](./images/neza-a-step-05-33.png)
![](./images/neza-a-step-05-34.png)
![](./images/neza-a-step-05-35.png)
![](./images/neza-a-step-05-36.png)
![](./images/neza-a-step-05-37.png)
![](./images/neza-a-step-05-38.png)
![](./images/neza-a-step-05-39.png)

## Hardware Connections
---
Connect two [motors](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 and M2 port and the [line-tracking sensor](https://www.elecfreaks.com/planetx-tracking.html) on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). ![](./images/neza-a-case-05-03.png)

## Programming
---
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html)

Import the libraries and the subsidiary libraries of [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html) and then import the libraries of the [line-tracking sensor](https://www.elecfreaks.com/planetx-tracking.html):  [PlanetXTracking-main.zip](https://github.com/elecfreaks/PlanetXTracking/archive/refs/heads/main.zip)
Download and import the self-defined library connections for [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html): [RJPins-main.zip](https://github.com/elecfreaks/RJPins/archive/refs/heads/main.zip)

### Sample Projects:

```
// Language ArduinoC
#include <NezhaA.h>
#include <RJPins.h>
#include <PlanetXTracking.h>

PlanetXTracking trackingJ1(J1);    //Create an instance of PlanetXTracking category
NezhaA nezha;    /Create an instance of NezhaA category

void setup() {
  nezha.begin();    //Initiliaze the buzzer, motor, servo and light
}

void loop() {
  if (trackingJ1.isTracked(Right)) {
    nezha.setMotorSpeed(M1, 0);    //Set the speed of the motor connecting to M1 at 0%
    nezha.setMotorSpeed(M2, 15);    //Set the speed of the motor connecting to M2 at 15%
  }
  if (trackingJ1.isTracked(Left)) {
    nezha.setMotorSpeed(M1, 15);    //Set the speed of the motor connecting to M1 at 15%
    nezha.setMotorSpeed(M2, 0);    //Set the speed of the motor connecting to M2 at 0%
  }  
}
```

### Result
After powering on, the car drives along with the map. 

