# case 04 trimpot 

## Introduction ##
---
The trimpot is a common pressure regulation component. In this case, we are going to read output voltage of the trimpot and show the voltage with a bar graph in 5*5 LED allay of micro:bit. 
## Hardware Connect ##
---

![](./images/LMsve7H.png)
- Connect circuit as above picture and put 2 AAA batteries to the batteries pack.

## Principles of Circuits ##
---
![](./images/VFmWZkG.png)

The GND of slot on micro:bit is into innards of batteries' GND to generate current loop.


## Introduction of Components ##
---
### Trimpot ###
- The trimpot is a pressure regulation component which included a resistance and a slide system. The resistance measured varies based on the movement of a knob or slider between the middle terminal and outer terminals. 
- There is a 10KΩ trimpot on the experiment box. When it turns left, it will be 0Ω; when it turns right, it will be 10KΩ.

![](./images/jHZQhOu.png)

## Software
---
### Step 1

- Click [makecode https://makecode.microbit.org/#](https://makecode.microbit.org/#)。

- Click on "New Project" and set a new Project.

![](./images/t34k5Zb.png)

### Step 2

![](./images/3Ekc31T.png)

- Snap plot bar graph into the forever to show a bar graph.（A bar graph is a kind of table which can show number by diffrent lengths.）

- "analog read pin" is to read a signal of a pin.（0~1023）

### Program

- Program link：[https://makecode.microbit.org/_VewWgwe8HVT1](https://makecode.microbit.org/_VewWgwe8HVT1)

- You also could directly download program by visiting website as below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_VewWgwe8HVT1" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


## Result
---
- Rotate the trimpot, the height of the bar graph will change.

![](./images/WDagGas.gif)

## think
---
- Is the trimpot could be a fixed resistance？

## Questions
---


## More Information 
---

