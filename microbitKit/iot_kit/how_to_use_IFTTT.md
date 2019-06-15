# The second part: Use the IoT kit to male a temperature alarm through Thingspeak and IFTTT.

## How to Send Temperature Threshold Value Alarm Email via IFTTT
---
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_01.jpg)
- In the article [How to Send Micro:bit Data to ThingSpeak IoT Platform](https://www.elecfreaks.com/12224.html), we have talked about how to use micro:bit to upload data to Thingspeak IoT platform. In this article, we will talk about how to use IFTTT to send micro:bit temperature thresholod value alarm email.
- What is IFTTT?
- IFTTT is the abbreviation of "if this then that". In fact, it causes a series of chain reaction to your website behaviour with the goal of "Put the internet to work for you", which brings you more convinience in usage. IFTTT aims to help people take advantage of public APIs of different websites in order to link websites(like Facebook、Twitter,etc.) or Apps together to complete your task. Thus, everyone can become a programer of the whole Internet without writing a program. IFTTT connects all kinds of information through process and then centrally present your desired information to you, which solves the problem of miscellaneous information and receive or focus on important information. According to IFTTT, the operation of "this" is called "Trigger", that is to say your behaviour in a certain website; while "that" means another behaviour "action" caused by the chain reaction. Those triggers and actions all based on a certain website, which is called "channel" in IFTTT. The whole "if this then that" action is defined to be "Task". Let me explain it to you with an example. In IFTTT, users can realize website chain reaction through creating and implementing a "Task". For example, if you have just uploaded your temperature data to Thingspeak using micro:bit, when the temperature arrives at a threshold value, it will activate the trigger so that to implement your designated action: send an email to your mail box.
Send micro:bit Temperature Alarm Email via IFTTT
First of all, please make sure that you have uploaded your temperature data from micro:bit to Thingspeak successfully. If you don't know how to do that, you can read this article for help. 
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_02.png)

## Step 1: Register an IFTTT Account
---
Log in IFTTT. If you don't have an account, please register one first.
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_03.png)
 

## Step 2: IFTTT Webhooks Setting

Create an Applet.
---
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_04.png)

Click on "this". 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_05.png)

Search for "webhooks".

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_06.png)

Choose trigger. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_07.png)

Name this task. Here we call it "microbit_temperature_alarm". 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_08.png)

Once we have completed trigger setting, click on "that". 
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_09.png)

Search for "email". 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_10.png)

Fill in your email contents and pay attention to the format showed, among which {{}} allows us to extract datas with the same name from Web Request and then forward it to the email.
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_11.png)

Completed. 
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_12.png)

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_22.png)

Click on "Documentation". 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_13.png)

This link is the link of web request. It is very important in the Thingspeak setting later on. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_14.png)

## Step 3: Thingspeak Setting
---
Before you do this, you must have uploaded your temperature data from micro:bit to Thingspeak. If you don't know how to do it, just read this acticle. Firstly, create a a new ThingHTTP service. 

![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_15.png)

Here's the setting of connection with IFTTT: 

 ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_16.png)

Note:
URL is the link of web request, which has to include a Private Key provided by IFTTT.
Content type must be JSON, because the expected format od IFTTT Maker Channel is JSON.
Within Body, you can invoke any data in Channel. This is the data that is going to be sent to IFTTT with the format as follow: {"value1":"%%channel_138112_field_1%%"}
For more details about ThingHTTP App, please refer to https:[//ww2.mathworks.cn/help/thingspeak/thinghttp-app.html](https://ww2.mathworks.cn/help/thingspeak/thinghttp-app.html). In the last, create a React service. 

 ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_17.png)

For more details about React APP, please refer to https://ww2.mathworks.cn/help/thingspeak/react-app.html.
### Step 4: Test
Till this step, you have already completed all of settings. Now let's test it! If the temperature has not arrived 30 degrees yet, you can hold micro:bit with your hands to improve its temperature.
 
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_18.png)

We can see from the data of Thingspeak channel that the temperature has surpassed 30m degrees. 
 ![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_19.png)

Check your email box and see if you have received an email from IFTTT! 
![](https://raw.githubusercontent.com/elecfreaks/learn-cn/master/microbitKit/iot_kit/images/case_ifttt_20.png)

