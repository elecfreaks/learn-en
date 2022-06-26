# Case 08: A Big Beetle

## Purpose
---
Make a big beetle with [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html).

![](./images/neza-a-case-08-01.png)

## Purchse
---
 [NezhaA Inventor's Kit](https://www.elecfreaks.com/elecfreaks-nezha-a-inventor-s-kit-for-arduino.html)

## Materials Required
---
![](./images/neza-a-case-08-02.png)

## Assembly Steps
---
![](./images/neza-a-step-08-01.png)
![](./images/neza-a-step-08-02.png)
![](./images/neza-a-step-08-03.png)
![](./images/neza-a-step-08-04.png)
![](./images/neza-a-step-08-05.png)
![](./images/neza-a-step-08-06.png)
![](./images/neza-a-step-08-07.png)
![](./images/neza-a-step-08-08.png)
![](./images/neza-a-step-08-09.png)
![](./images/neza-a-step-08-10.png)
![](./images/neza-a-step-08-11.png)
![](./images/neza-a-step-08-12.png)
![](./images/neza-a-step-08-13.png)
![](./images/neza-a-step-08-14.png)
![](./images/neza-a-step-08-15.png)
![](./images/neza-a-step-08-16.png)
![](./images/neza-a-step-08-17.png)
![](./images/neza-a-step-08-18.png)
![](./images/neza-a-step-08-19.png)
![](./images/neza-a-step-08-20.png)
![](./images/neza-a-step-08-21.png)
![](./images/neza-a-step-08-22.png)
![](./images/neza-a-step-08-23.png)
![](./images/neza-a-step-08-24.png)
![](./images/neza-a-step-08-25.png)
![](./images/neza-a-step-08-26.png)
![](./images/neza-a-step-08-27.png)
![](./images/neza-a-step-08-28.png)
![](./images/neza-a-step-08-29.png)
![](./images/neza-a-step-08-30.png)
![](./images/neza-a-step-08-31.png)
![](./images/neza-a-step-08-32.png)
![](./images/neza-a-step-08-33.png)
![](./images/neza-a-step-08-34.png)
![](./images/neza-a-step-08-35.png)
![](./images/neza-a-step-08-36.png)
![](./images/neza-a-step-08-37.png)
![](./images/neza-a-step-08-38.png)
![](./images/neza-a-step-08-39.png)
![](./images/neza-a-step-08-40.png)
![](./images/neza-a-step-08-41.png)
![](./images/neza-a-step-08-42.png)
![](./images/neza-a-step-08-43.png)
![](./images/neza-a-step-08-44.png)
![](./images/neza-a-step-08-45.png)
![](./images/neza-a-step-08-46.png)
![](./images/neza-a-step-08-47.png)
![](./images/neza-a-step-08-48.png)
![](./images/neza-a-step-08-49.png)
![](./images/neza-a-step-08-50.png)
![](./images/neza-a-step-08-51.png)
![](./images/neza-a-step-08-52.png)
![](./images/neza-a-step-08-53.png)
![](./images/neza-a-step-08-54.png)
![](./images/neza-a-step-08-55.png)
![](./images/neza-a-step-08-56.png)
![](./images/neza-a-step-08-57.png)
![](./images/neza-a-step-08-58.png)
![](./images/neza-a-step-08-59.png)
![](./images/neza-a-step-08-60.png)
![](./images/neza-a-step-08-61.png)
![](./images/neza-a-step-08-62.png)



## Hardware Connections
---
Connect two [motors](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to M1 and M2 port,  the [ultrasonic sound sensor](https://www.elecfreaks.com/planetx-ultrasonic.html) to J1 port and  the [line-tracking sensor](https://www.elecfreaks.com/planetx-tracking.html) on J2 port on [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html). 

![](./images/neza-a-case-08-03.png)

## Programming
---
### Prepare the programming

Steps for preparation please refer to: [Arduino 3 in 1 Breakout Board](https://www.elecfreaks.com/learn-en/Arduino-3-in-1-box/Arduino-3-in-1-box.html)

Import the libraries and the subsidiary libraries of [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html) and then import the libraries of the [line-tracking sensor](https://www.elecfreaks.com/planetx-tracking.html):  [PlanetXTracking-main.zip](https://github.com/elecfreaks/PlanetXTracking/archive/refs/heads/main.zip)

Import the libraries and the subsidiary libraries of [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html) and then import the libraries of the [ultrasonic sound sensor](https://www.elecfreaks.com/planetx-ultrasonic.html):  [PlanetXUltrasonic-main.zip](https://github.com/elecfreaks/PlanetXUltrasonic/archive/refs/heads/main.zip)
Download and import the self-defined library connections for [Nezha-A master box](https://www.elecfreaks.com/arduino-3-in-1-master-control-box.html): [RJPins-main.zip](https://github.com/elecfreaks/RJPins/archive/refs/heads/main.zip)

### Sample Code: 

```
// Language ArduinoC
#include <NezhaA.h>
#include <RJPins.h>
#include <PlanetXTracking.h>
#include <PlanetXUltrasonic.h>

PlanetXTracking trackingJ2(J2);    //Create an instance of PlanetXTracking category
NezhaA nezhaa;    //Create an instance of Nezha category
PlanetXUltrasonic ultrasonicJ1(J1);    // Create an instance of PlanetXUltrasonic category
int distance;    //Create a variable of int distance

void setup() {
  nezhaa.begin();    //Initiliaze the buzzer, motor, servo and light
}

void loop() {
  distance = (ultrasonicJ1.getDistance());    //Set the detected value from ultrasonic sound sensor as the variable distance 
  if (distance > 3 && distance < 20) {    //Judge if the variable is over 3 and below 20
    nezhaa.setMotorSpeed(M1, 0);    //Set the speed of the motor connecting to M1 at 0%
    nezhaa.setMotorSpeed(M2, 0);    //Set the speed of the motor connecting to M2 at 0%
  } 
  else {
    if (trackingJ2.isTracked(Right)) {
      nezhaa.setMotorSpeed(M1, 0);    //Set the speed of the motor connecting to M1 at 0%
      nezhaa.setMotorSpeed(M2, 20);    //Set the speed of the motor connecting to M2 at 20%
    }
    if (trackingJ2.isTracked(Left)) {
      nezhaa.setMotorSpeed(M1, 20);    //Set the speed of the motor connecting to M1 at 20%
      nezhaa.setMotorSpeed(M2, 0);    //Set the speed of the motor connecting to M2 at 0%
    }  
  }  
}
```

### Result
After powering on, the beetle walks along with the line and it stops while it detects the obstacles. 
