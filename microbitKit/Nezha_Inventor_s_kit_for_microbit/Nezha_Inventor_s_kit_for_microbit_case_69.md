# Case 69: The Trimpot Remote Control Car
## Introduction

Use **[Nezha 48 IN 1 Inventor's Kit](https://www.elecfreaks.com/nezha-inventor-s-kit-for-micro-bit-without-micro-bit-board.html)** with [ELECFREAKS Interactive Coding Accessories Pack](https://shop.elecfreaks.com/products/elecfreaks-interactive-coding-accessories-pack)
to make a remote control car through the potentiometer, which includes two blocks parts of the remote controller and the car. 

![](./images/neza-inventor-s-kit-case-69-01.png)

## Case Building

### Materials Required

[ELECFREAKS micro:bit Nezha 48 IN 1 Inventor's Kit ](https://shop.elecfreaks.com/products/elecfreaks-micro-bit-nezha-48-in-1-inventors-kit-without-micro-bit-board)

[ELECFREAKS Interactive Coding Accessories Pack](https://shop.elecfreaks.com/products/elecfreaks-interactive-coding-accessories-pack)


### Structure Building

In this case we will make two block structures, the `remote control car` and `remote control handle` respectively.

**Remote control car building steps**

Parts list

![](./images/neza-inventor-s-kit-case-69-02.png)

The structure is built as shown in the figure:

![](./images/neza-inventor-s-kit-step-69-01.png)

![](./images/neza-inventor-s-kit-step-69-02.png)

![](./images/neza-inventor-s-kit-step-69-03.png)

![](./images/neza-inventor-s-kit-step-69-04.png)

![](./images/neza-inventor-s-kit-step-69-05.png)

![](./images/neza-inventor-s-kit-step-69-06.png)

![](./images/neza-inventor-s-kit-step-69-07.png)

![](./images/neza-inventor-s-kit-step-69-08.png)

![](./images/neza-inventor-s-kit-step-69-09.png)

![](./images/neza-inventor-s-kit-step-69-10.png)

![](./images/neza-inventor-s-kit-step-69-11.png)

![](./images/neza-inventor-s-kit-step-69-12.png)

![](./images/neza-inventor-s-kit-step-69-13.png)

![](./images/neza-inventor-s-kit-step-69-14.png)

![](./images/neza-inventor-s-kit-step-69-15.png)

![](./images/neza-inventor-s-kit-step-69-16.png)

![](./images/neza-inventor-s-kit-step-69-17.png)

![](./images/neza-inventor-s-kit-step-69-18.png)

![](./images/neza-inventor-s-kit-step-69-19.png)

![](./images/neza-inventor-s-kit-step-69-20.png)



Build completion:

![](./images/neza-inventor-s-kit-step-69-21.png)

**Remote control handle building steps**

Parts list

![](./images/neza-inventor-s-kit-case-69-03.png)


The structure is built as shown in the figure:

![](./images/neza-inventor-s-kit-step-69-22.png)

![](./images/neza-inventor-s-kit-step-69-23.png)

![](./images/neza-inventor-s-kit-step-69-24.png)

![](./images/neza-inventor-s-kit-step-69-25.png)

![](./images/neza-inventor-s-kit-step-69-26.png)

![](./images/neza-inventor-s-kit-step-69-27.png)

![](./images/neza-inventor-s-kit-step-69-28.png)

![](./images/neza-inventor-s-kit-step-69-29.png)

![](./images/neza-inventor-s-kit-step-69-30.png)

![](./images/neza-inventor-s-kit-step-69-31.png)

![](./images/neza-inventor-s-kit-step-69-32.png)




Finished Picture:

![](./images/neza-inventor-s-kit-step-69-33.png)



### Connection Diagram

**Remote control handle reference**

Connect two [Potentiometers](https://www.elecfreaks.com/planetx-trimpot.html) to J1 and J2 port， and the [Rainbow](https://www.elecfreaks.com/geekservo-motor-2kg-compatible-with-lego.html) to  J3 port on [Nezha Breakout Board](https://www.elecfreaks.com/nezha-breakout-board.html).

![](./images/neza-inventor-s-kit-case-69-04.png)

**Remote control car reference**

Connect two [Potentiometers](https://www.elecfreaks.com/planetx-trimpot.html) to M1 port and M2 port on [Nezha Breakout Board](https://www.elecfreaks.com/nezha-breakout-board.html) .

![](./images/neza-inventor-s-kit-case-69-05.png)

## MakeCode Programming

### Step1

Click "extensions" in the MakeCode drawer.

![](./images/neza-inventor-s-kit-case-37-04.png)

For programming the potentiometer and the rainbow，we need to add an extension library. Search with "PlanetX" in the dialog box to download this library.

![](./images/neza-inventor-s-kit-case-37-05.png)

For programming the Nezha expansion board, we need to add an expansion library. Search with "Nezha" in the dialog box to download it.

![](./images/neza-inventor-s-kit-case-37-06.png)

*Notice*: If you met a tip indicating that some codebases would be deleted due to incompatibility, you may continue as the tips say or create a new project in the menu.

### Step 2

**Remote control cart program*

### Write the program as the picture suggests

![](./images/neza-inventor-s-kit-case-69-06.png)

### Reference

Link: [https://makecode.microbit.org/_4E0ayHcEHXgL](https://makecode.microbit.org/_4E0ayHcEHXgL)

You may also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_4E0ayHcEHXgL" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

Remote control handle program

### Write the program as the picture suggests

![](./images/neza-inventor-s-kit-case-69-07.png)

### Reference
link: [https://makecode.microbit.org/_51MbzXhRTDvq](https://makecode.microbit.org/_51MbzXhRTDvq)

You may also download it directly:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_51MbzXhRTDvq" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

### Result
The two potentiometers can respectively remote control the left and right wheels of the cart, through the rainbow light ring on the handle shows the speed difference between the two wheels of the cart, when the speed of the right wheel of the cart is higher, the left side of the rainbow light ring on the handle lights up, then the cart turns left; when the speed of the left wheel of the cart is higher, the right side of the rainbow light ring on the handle lights up, then the cart turns right; when the speed of the wheels on both sides of the cart does not differ much, the three lights in the middle of the rainbow ring light up, and then the car moves forward.

![](./images/neza-inventor-s-kit-case-69.gif)

