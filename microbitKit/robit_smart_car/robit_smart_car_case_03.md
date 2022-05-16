# case 06 Rainbow LED

## Our Goal  
---  
- Use LEDs on robit to make dazzling colorful light.   


## Material Needed   
---  

- 1 x Robit
- 1 x Mbot Car  


## Background Knowledge  
---  

### Rainbow LED  

[RGB](https://en.wikipedia.org/wiki/RGB_color_model) color model is a color standard in the industry. It can be used to create a variety of colors through the change of RGB channels and their interactive mixture. RGB stands for red, green and blue. This standard has almost included all kinds of colors that are visually perspective by human eyes. It is one of the most widely used color system. 

Rainbow LED is a kind of LED. It has integrated red, green and blue LED into one component. We all know that the three primary colors of light are red, green and blue. With different color combination, we can synthesize the color of all things. Similarly, by combining different RGB brightness of light, we can also create an infinite number of colors.    

The LEDs on Robit are WS2812b LEDs, which have similar outlook with 5050 bead. Each bead is a pixel. The picture below is a single bead that has four pins.  

![](./images/um2QZl8.png)  


## Hardware Connection  
---  

Two rainbow LEDs onboard are connected to P12 on micro:bit.   

![](./images/yOJCtFk.png)  

![](./images/VB66oQ7.jpg)  


## Software   
---  
[Microsoft Makecode](https://makecode.microbit.org/#)  


## Programming   
---  

### Step 1  

Click **Advanced** in the code drawer of MakeCode to see more code options.  

![](./images/LjMR5IU.png)  

To program for robit, we have to add a package. Find **Add Package** in the bottom of code drawer and click it. This will pop up a dialogue box. Search **Robit** and then click to download this package. 

![](./images/ISZ6w26.png)  

***Note:*** If you get a hint that some packages will be deleted due to the problem of incompatibility, you can either follow the prompts, or create a new project in the project menu.

### Step 2  

When start, we have to create a variable item to assign values to LEDs. Let's define its initial color to be 0.

Then create a forever loop and make variable item increase by 5 during each circulation. If the value of item equals to 360, then set it to be 0 to restart loop.

![](./images/UG17sXN.png)  

***Note:*** Picture below is the detailed code explain of LED.  

![](./images/fojUByb.png)  
 

## Program   
---  

You can see the whole program from the link here: [https://makecode.microbit.org/_DLqKtp38EVro](https://makecode.microbit.org/_DLqKtp38EVro)

Or you can download it from the page below.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_DLqKtp38EVro" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


## Result  
---
We can see the color of LED light is changing circularly.    

![](./images/9KOWt1T.gif)  


## Think   
---  

How to make the color change swiftly instead of smooth change?  


## FAQ  
---  

Q: How to change RGB flash speed?  

A: Renew the change rate of the variable item.  

