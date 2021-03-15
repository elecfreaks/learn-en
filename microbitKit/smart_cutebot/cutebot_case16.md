# AI Lens Line-tracking Kit

## Purpose
---
- Use the Cutebot and the AI lens to achieve the line tracking function. 

## Materials required

---
- 1 × [Cutebot V3.0](https://www.elecfreaks.com/store/cute-bot.html)

- 1 × [Cutebot lithium battery pack](https://www.elecfreaks.com/cutebot-lithium-battery-pack.html)

- 1 × [AI Lens Kit](https://www.elecfreaks.com/elecfreaks-smart-ai-lens-kit.html)

  *Note: The AI Lens kit works with Cutebot V3.0 only(You can see the version number printed on the baseboard).*

![](./images/cutebot-16-04.png)

## Connections:

---
### Steps to install the lithium battery pack: 

![](./images/cutebot-step-01.png)

Assembly steps for bricks:

Parts list:

![](./images/cutebot-step-02.png)

Steps of build-up:

![](./images/cutebot-step-03.png)

![](./images/cutebot-step-04.png)

![](./images/cutebot-step-05.png)

![](./images/cutebot-step-06.png)

![](./images/cutebot-step-07.png)

![](./images/cutebot-step-08.png)

![](./images/cutebot-step-09.png)



### Connections of the AI Lens: 
Connect the RJ11 cable with the AI Lens and the other end in Dupont connection to the circled place in the below picture (make sure you connect to the right connections).

![](./images/cutebot-step-10.png)

*Tips: the bricks holder here is flexible to be adjusted, we may manually adjust the angles of the AI lens to meet the requirements of the functions that you want to achieve.*

## Software Platform:
---
[MicroSoft MakeCode](https://makecode.microbit.org/#)

## Programming

---
### Step 1
- Click “Advanced” in the drawer to see more choices.

![](./images/cutebot-pk-1.png)

- We need to add a package for programming. Click “Extensions” in the bottom of the drawer and search with “cutebot” in the dialogue box to download it.

  ![](./images/cutebot-pk-11.png)

- We need to add a package for programming the AI lens kit. Click “Extensions” in the bottom of the drawer and search with “https://github.com/elecfreaks/pxt-PlanetX-AI” in the dialogue box to download it.

![](./images/cutebot-pk-12.png)

*Note: If you met a tip indicating that the codebase will be deleted due to incompatibility, you may continue as the tips say or build a new project in the menu.*

###  Step 2

- In the “on start” brick, initialize the AI lens and switch the function to the line tracking mode, set the micro:bit to display the appointed icon.

![](./images/case-16-01.png)

- In the “forever” brick, set to get one image form the AI lens and judge the deviation direction of the line on the image. If it deviates to the left side, it means the car deviates to the right, we should set the speed of the left wheel at the speed of 10% and the right at 40% to make the car turn left and go to the right way; if the line deviates to the right side, it means the car deviates to the left side, now we should set the speed of the right wheel at the speed of 10% and the left at 40% to make the car turn right and go to the right way; or we may set the speed of both wheels at 20% and the car moves forward with the line. 

![](./images/case-16-02.png)

### Code

![](./images/case-16-03.png)

Link: [https://makecode.microbit.org/_hcy8YeM87AVd](https://makecode.microbit.org/_hcy8YeM87AVd)

You may also download it directly below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:https://makecode.microbit.org/_hcy8YeM87AVd" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin">
</iframe>
</div>  
---

## Result 
---
- The Cutebot car moves along with the black line.

![](./images/case-16-04.gif)


## Exploration
---

## FAQ
---
## Relevant Files
---
