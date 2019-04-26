#  case 10 PADDLEBALLSUPERSMASHEM 

![](./images/ngNx9A3.jpg)  

Learn to program a simple yet fun game on a 5 by 5 display, using JavaScript! PADDLEBALLSUPERSMASHEM may bear unintentional similarities to other, more graphical, games.  


## Step 0 – Pre Build Overview      
---  

In this project, we will create a simple game, in which you bounce a ball against a wall. If you miss, you die. Too bad. For those of you who appreciate a challenge, the game increases in difficulty with each level!  


## Goals      
---  

- Get to know more about the microbit microcomputer  
- Learn how to program a simple game  
- Consider all cases  


## Material     
---   

- 1 x BBC micro:bit
- 1 x Micro USB cable  

![](./images/Im2BXNd.jpg)  


## How to Make    
---    

### Step 1: Components     

First of all, plug the microbit microcomputer into your own computer. No other components are required.  

![](./images/fqrpqTW.jpg)  


### Step 2： Pre-coding    

We will add a package of code to enable us to use our kit components. Click on “Advanced” in the Code Drawer to see more code section and look at the bottom of the Code Drawer for “Add Package”.    

![](./images/I2L5019.jpg)      

This will open up a dialog box. Search for "tinker kit" and then click on it to download this package.    

![](./images/8a7kDKF.png)     

Note: If you get a warning telling you some packages will be removed because of incompatibility issues, you should either follow the prompts or create a new project in the Projects file menu.     


### Step 3: Coding      

![](./images/SfkOKmO.png)    

First of all, define your variables! We are going to need many variables to store the location, speed and direction of the ball, the length and position of the paddle, and last but not least, your score!    

![](./images/oYBRGY9.png)   

Next, we will program the functions that control the paddle. xb represents the position of the first pixel of the paddle from the left, and yb represents the length of the paddle. The left and right functions control xb and shift the paddle, and the board function prints the paddle on the screen.  

![](./images/lQ0drJR.png)  

Next, we include the function that controls when the ball moves. At the beginning, the ball moves every second but as you advance, the ball moves at shorter and shorter intervals! How exciting!   

![](./images/c6jUmNb.png)  

We now program the functions that control how the ball interacts with its surroundings. When the ball hits the side, its horizontal movement is reversed but its vertical movement remains the same. When the ball hits the ceiling, it can rebound in any direction, to make the game more fun.   

![](./images/MrcNyKJ.png)  

Most importantly, we need to see if the ball hits the paddle. If it misses, you lose, displaying your score! If it doesnt miss, the ball will also rebound in a random direction, and the difficulty of the game will increase.  

![](./images/WIXWKV0.png)  

Lastly, we have a for loop which acts as a clock so that the ball keeps moving. Also, we have the onButtonPressed() functions that move the paddle.  

Save your tired fingers and download the code from the link below.   

[https://makecode.microbit.org/63331-03858-42547-81536](https://makecode.microbit.org/63331-03858-42547-81536)   

Or you can download from this page.   

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:63331-03858-42547-81536" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Step 4: Using It    

![](./images/yARLugY.jpg)   

Just connect the microcontroller to your computer, and run the program! Easy!  

![](./images/cV3q2Ar.jpg)  

If you score more than 12 points, you will be rewarded with a smiley face! Otherwise, the program may not be very pleased…   

### Step 5: Success!     

Voila! You have now programmed PADDLEBALLSUPERSMASHEM on a 5 by 5 display. You should be proud of yourself.     
