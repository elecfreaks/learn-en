# Octopus MG811 CO2 Gas Sensor

## Introduction
---

Octopus MG811 CO2 Gas Sensor is a CO2 electronic brick in our OCTOPUS series, the basic design for the outlook, PCB fixing holes and connections are the same with them. 

The higher the CO2 concentration is, the lower the output voltage would be. The users can read the CO2 value easily after checking our brochures and coding samples. 

The CO2 probe is made with industrial grade which is high allergic to CO2 and anti-interference to alcohol and CO.  It is of high performance and quick response with loaded signal amplification circuit even in different temperature and humidity environment.  Besides, the heating circuit on-board helps to convert to stable 6V voltage from 5V directly that improves the adaptability of the module.  

**Caution:**

- The module belongs to electrochemistry CO2 and the probe heats itself when working, please do not touch in case getting hurt.
- Please make a seal preservation while the sensor is not in use in case the probe getting "poisoned" due to the long time exposure in the air or you have to heating continuously another 48 hours to activate it!
- The MG-811 probe belongs to the category of  electrochemistry sensor, please make a proving operation for it before using to get an accurate value. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitOctopus/sensor/images/04100_00.jpg)

## Characteristic
---
- Working voltage of  the probes: 6v
- With  booster circuit inbuilt, it supports input DC 3.7~5V and the current over 500mA. 
- OCTOPUS electronic bricks.
- Easy connection.

## Parameter
---
- Item: Octopus MG811 CO2 Gas Sensor
- SKU：EF04100
- Working Voltage: DC 3.7~5v
- Connection Mode: G-GND，V-VCC，S-pin signals 
- Size: 31 * 48mm
- Net Weight: 9.6g

## Outlook and Dimension:
---

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitOctopus/sensor/images/04100_02.png)

## Quick to Start  
---
### Hardware Connection

The module connects to the A0 of the Arduino UNO through a Dupont wire with a best fastener, the Arduino main board much be powered with extra connection(7.5V-9V). 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitOctopus/sensor/images/04100_01.jpg)

### Software Programming

#### Proving Operation

The MG-811 probe belongs to the category of  electrochemistry sensor, please make a proving operation for it before using to get an accurate value. 
The probes heat itself after giving stable power supply. Please put the module to a place in fresh air and heat for 48 hours continuously. Please measure the output voltage(unit: V) of the module and divides with 8.5, the final value should be filled into the macro definition of the code: 

```
#define ZERO_POINT_VOLTAGE (Revise as: Voltage(V)/8.5) 
```

For example: if the voltage tested by the multimeter is 2.4V, then we use 2.4/8.5=0.282, and we should revise them as below:

```
#define ZERO_POINT_VOLTAGE (0.282) 
```

After revising, please upload it to Arduino main board and you can use it to test your own projects now. 

#### Coding Samples 
```
/*******************Demo for MG-811 Gas Sensor Module V1.1*****************************
************************************************************************************/

/************************Hardware Related Macros************************************/
#define         MG_PIN                       (A0)     //define which analog input channel you are going to use
#define         DC_GAIN                      (8.5)   //define the DC gain of amplifier

/***********************Software Related Macros************************************/
#define         READ_SAMPLE_INTERVAL         (50)    //define how many samples you are going to take in normal operation
#define         READ_SAMPLE_TIMES            (5)     //define the time interval(in milisecond) between each samples in 
                                                     //normal operation

/**********************Application Related Macros**********************************/
//These two values differ from sensor to sensor. user should derermine this value.
#define         ZERO_POINT_VOLTAGE           (0.220) //define the output of the sensor in volts when the concentration of CO2 is 400PPM
#define         REACTION_VOLTGAE             (0.030) //define the voltage drop of the sensor when move the sensor from air into 1000ppm CO2

/*****************************Globals***********************************************/
float           CO2Curve[3]  =  {2.602,ZERO_POINT_VOLTAGE,(REACTION_VOLTGAE/(2.602-3))};   
                                     //two points are taken from the curve. 
                                     //with these two points, a line is formed which is
                                     //"approximately equivalent" to the original curve.
                                     //data format:{ x, y, slope}; point1: (lg400, 0.324), point2: (lg4000, 0.280) 
                                     //slope = ( reaction voltage ) / (log400 –log1000) 

void setup()
{
   Serial.begin(9600);              //UART setup, baudrate = 9600bps
   Serial.print("MG-811 Demostration\n");                
}

void loop()
{
    int percentage;
    float volts;

    volts = MGRead(MG_PIN);
    Serial.print( "SEN0159:" );
    Serial.print(volts); 
    Serial.print( "V           " );

    percentage = MGGetPercentage(volts,CO2Curve);
    Serial.print("CO2:");
    if (percentage == -1) {
        Serial.print( "<400" );
    } else {
        Serial.print(percentage);
    }

    Serial.print( "ppm" );  
    Serial.print("\n");

    delay(500);
}

/*****************************  MGRead *********************************************
Input:   mg_pin - analog channel
Output:  output of SEN-000007
Remarks: This function reads the output of SEN-000007
************************************************************************************/ 
float MGRead(int mg_pin)
{
    int i;
    float v=0;

    for (i=0;i<READ_SAMPLE_TIMES;i++) {
        v += analogRead(mg_pin);
        delay(READ_SAMPLE_INTERVAL);
    }
    v = (v/READ_SAMPLE_TIMES) *5/1024 ;
    return v;  
}

/*****************************  MQGetPercentage **********************************
Input:   volts   - SEN-000007 output measured in volts
         pcurve  - pointer to the curve of the target gas
Output:  ppm of the target gas
Remarks: By using the slope and a point of the line. The x(logarithmic value of ppm) 
         of the line could be derived if y(MG-811 output) is provided. As it is a 
         logarithmic coordinate, power of 10 is used to convert the result to non-logarithmic 
         value.
************************************************************************************/ 
int  MGGetPercentage(float volts, float *pcurve)
{
   if ((volts/DC_GAIN )>=ZERO_POINT_VOLTAGE) {
      return -1;
   } else { 
      return pow(10, ((volts/DC_GAIN)-pcurve[1])/pcurve[2]+pcurve[0]);
   }
}
```


### Result

Open the serial monitor and you will get the concentration of the CO2 around you after 5 minutes. 

## FAQ
