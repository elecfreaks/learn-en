# Excel and micro:bit

## Excel and micro:bit - Hacking for fun and creativity!

### The Experiment
---
For the purpose of this first entry-level experiment, lets agree that the goal would be to have some basic sensor data collected using the micro controller and then visualized in Excel.


To achieve that, we will go thru four steps:

1. We will program the controller to collect some sensor data and send it over its’ built in serial  communication port.
2. We will connect the micro:bit to the PC’s serial port.
3. We will write a small program in Excel that reads the data from the serial port into the grid.
4. Visualize it, live! This is why we’re here for… :-)

![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/13765i883EB36245B45F26/image-size/large?v=1.0&px=999)

**The Experiment Flow - Data flows from Micro:Bit to Excel**

These are the basic building blocks and it’s pretty simple to get started. You can do it as your fun weekend project!


Once you get going, the sky is the limit. You can expand to control the device, interact with other devices using the programmable pins, control the LEDs, respond to the buttons, etc. Just use your imagination and creativity, or get yourself inspired by this [list of Micro:Bit project ideas!](http://microbit.org/ideas/)

It’s worth mentioning that while this blog focuses on the micro:bit, it’s totally possible to envision doing the same with your favorite controller of choice. So, if you’re a fan of Arduino, for example, feel free to adapt the experiment, and even better – share it back with this community!


### First thing’s first: Programming the micro:bit
Programming the micro:bit is the easiest thing you’ll ever do. Microsoft actually has a web-based development environment ready for you (Microsoft is one of the founding partners of the micro:bit).


All you have to do is, go to [www.makecode.com](http://www.makecode.com/), select the micro:bit as your device, and write a little program using a visual “Block-based” programming language.


The program we’ll write for this experiment will simply collect data from two sensors that we can easily play with – acceleration and light level, and send a sampling of the sensors over the serial communication port every 100ms.


It looks like this:

 ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/13766iFDD7F612BBF9EC83/image-size/large?v=1.0&px=999)

**The program that we'll run on the Micro:Bit**

`D:<light>,<acceleration>`


All you have to do now is load the program into your Micro:Bit. To do that, connect your micro:bit to the PC using a USB cable, which will make it appear like a removeable disk drive. Then download the HEX file from within the MakeCode environment and save it onto the device. A few seconds later, the program will start running.


To save you from having to re-type the program yourself, you can find a public copy of it [here](https://pxt.microbit.org/30666-98262-90183-87306).


### Connecting it to the PC

Now that we have our controller running and sending data, and before we try it out in Excel, it’s a good idea to verify that the PC can indeed see the incoming data stream.
To do that, you’ll need to follow the instructions on [this page](https://www.microbit.co.uk/td/serial-library), which basically means you need to do two things:

1. Install a driver, which will make the micro:bit “appear” as a serial port on your PC.
Test it with a serial communication terminal emulator.

2. You will need to configure the right COM port. On my environment, it was configured to COM3. The sample code in Excel assumes that, so if yours is different, you’ll need to modify the Excel code later on to reflect the right port.


Once you do that, you should see a stream of data that looks something like this inside your emulator:

 ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/13768i03054CCA134AD00F/image-size/medium?v=1.0&px=400)

**The incoming data flow - light level and acceleration**

Working? Time to move to the next step!

### Lets’ Excel! 

Now that we have a stream of incoming data, lets get it into Excel. The spreadsheet comprises of two parts – some VBA code that is used to communicate with the micro controller, and then some basic grid data manipulation functions which are used to break the data points and charts it. You can find a copy of the working spreadsheet [attached to this blog](https://techcommunity.microsoft.com/gxcuf89792/attachments/gxcuf89792/ExcelBlog/48.6/1/SensorVisualizer_BlogVersion.zip).


Assuming you want to build it yourself, or at least understand it fully, it’s time to pull up your sleeves and write some VBA code that will read the data from the serial port, and push it into the grid.


Because this is an endless stream of data, for the purpose of this experiment, we will iterate thru the last 30 data samples collected. Of course, once you get the idea, you can change it to accumulate forever (or at least till the sheet fills up), push the data into a data model, etc. For now, we’ll just iterate thru it, so whenever we reach the 30th row, we’ll roll back to the first one.


One more point: When reading from the serial communication port in VBA, the most reliable way to do that is to read byte-by-byte and not whole lines. There’s also some chance of losing some data (depending on speed of communications, speed of VBA execution, etc.), which is why I’ve added the “D:” prefix for each line. If the line we read doesn’t start with it, the line gets ignored as garbage data.


With no further ado, here’s a snippet from the main loop in the VBA code:
 
![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/13769iE0B5271D5697938C/image-size/large?v=1.0&px=999)

**The main communication read loop. You can find the code inside the attached workbook!**

few things to note in this code snippet:

 

1. We open the COM3: port at 115,200 baud (the speed at which the Micro:Bit sends data).
2. Reading happens a byte at a time, until end of line (char(13)) is detected.
3. Whenever a line is read, it gets pushed into the grid into the next row in a fixed column. Row 
numbers are fixed between 2-31 to keep this example simpler.
4. There is a flag used to stop reading. It’s triggered by a stop button (from a different Macro).

The best way to understand this code it is to run it in debug mode and step thru it, so go ahead and download the demo workbook and experiment!


**Moving on to “real” Excel**
Now that we have the data coming into the grid, we’re in the plain old good Excel formula and charting territory. Time to do something with the data we are collecting!


To keep things generic, the VBA scripts reads the data as-is into the grid, so Column “E” contains the actual data, as it arrived over the wire. In our case, it’s two numbers, comma-separated.


So, first thing we want to do is to break it up into two distinct values per row. The light level, and the acceleration value. I did that on purpose in the easy to read way – used the FIND formula to find the location of the “,” separator inside the incoming data, and then used NUMERVALUE and LEFT and RIGHT formulas to break the string apart and convert it into two numeric values.


Here is a bit more about the formulas I used to break down the values from the input data string:

  ` =FIND(",",E2,1)` : Finds the location of the first comma separator inside cell E2 (which contains the raw incoming string of comma-separated values).
  ` =NUMBERVALUE(LEFT(E2,F2-1))` : Takes the left side of the string, up to the comma location, and convert it to a number value. This gives us a number representing the light sensor value. Light values in the Micro:Bit range from 0 to 255.
   `=NUMBERVALUE(RIGHT(E2,LEN(E2)-F2))` : Similar to the previous formula, only taking the right side number, which is the acceleration value. Values can be on the X,Y or Z axis, or combined, and explained [here](https://pxt.microbit.org/reference/input/acceleration).


I also added a fixed “Row” column numbered 1-30, so that we will have an X axis for our charts.


The final piece of the puzzle – create two charts from the values. In both of them, the X axis is the row number, and the Y axis is the data coming in from the sensor (either light or acceleration).
This is what it looks like:

![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/13770i859D1310A25977A3/image-size/large?v=1.0&px=999)

**The end result - incoming data is visualized live!**

All you have to do now is click “Start” and see the data coming in and being charted live! Shake the device and the acceleration level jumps all over. Flash it with a flashlight or cover it with your hands and the light level chart reflects it. You’ve just built a cool programmable fidget toy with Excel!


From here on, you can of course implement your own logic to analyze the data and make this example do something real with the data, based on what you want to do.

