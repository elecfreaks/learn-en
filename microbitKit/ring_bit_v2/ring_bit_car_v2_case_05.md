# case 05 Crazy dance 

## Our Goal
---
- To make the Ring:bit car to dance in free style. 

## Requiered Materials
---
- 1 x Ring:bit Car

## Hardware Connect
---
- Connect the left wheel servo to P1 of the Ring:bit expansion board and the right wheel servo to P2.
![](./images/jBVHea8.png)

## Software
---
[makecode](https://makecode.microbit.org/#)

## Coding
---
### Step 1
- Click on "Advanced" in the MakeCode Drawer to see more code sections.

![](./images/2qCyzQ7.png)

- Search for “ringbitcar” and click on the ring:bit car package to add it to your project. (As below picture)

![](./images/1Wq2Mov.jpg)

Note：If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Project file menu.


### Step 2

- Snap the block `set left wheel at pin P1 right wheel at pin P2` to the `On start` block. 
- The port number is based on the actual servo connection port.
![](./images/igG5TVD.png)

### Step 3
- Snap blocks into `forever` block.
- Set an varieble to `left` and an variable to `right`.
- Generate a random number and assinment to the `left` and the `right`.

![](./images/2PPYJ0T.png)

### Step 4

- Set the left wheel speed to the variable left abd the right wheel speed to the variable right.
- Pause for one second.

![](./images/HSujBjF.png)


### Program

Program Link：[https://makecode.microbit.org/_PXXfa8FF5MWs](https://makecode.microbit.org/_PXXfa8FF5MWs)

If you don't want to type these code by yourself, you can directly download the whole program from the link below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_PXXfa8FF5MWs" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---


## Result
---
- The car runs at different speed.

![](./images/j6kX56N.jpg)

## Think
---
- How do you ensure the car moves at a slower speed constantly?

## Questions
---


## More Information 
---

