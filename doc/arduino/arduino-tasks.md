# Arduino tasks

## Table of Content

[Installation](#installation)    
[01 Video: Massimo Banzi: How Arduino is open-sourcing imagination]() 
[]() 
[]() 
[]() 
[]() 


[01 Arduino Experimenter's Guide for NodeJS](#01-arduino-experimenters-guide-for-nodejs)  
[02 Arduino with Electron UI Getting Started](#02-arduino-with-electron-ui-getting-started)  
[03 Arduino with Electron UI Button Pressing](#03-arduino-with-electron-ui-button-pressing)  
[04 Arduino with Electron UI Twisting](#04-arduino-with-electron-ui-twisting)  


___

## Installation

1. Download and install the arduino software https://www.arduino.cc/en/Main/Software

2. Open the Arduino IDE and select your board: Tools > Board > Arduino Genuino Uno

3. (windows) Select the port: Tools > Port. This is likely to be com3 or higher (Max Os 10) /dev/tty.usbmodem

4. Launch Arduino IDE and open the Firmata sketch via the menu: File > Examples > Firmata > StandardFirmataPlus
  * Select your Arduino board type (e.g. Arduino Uno) via Tools > Board
  * Select the port for your board via Tools > Serial Port > (the comm port of your Arduino)
  * Upload the program by selecting File > Upload  

5. Install johnny five:
  * Install Node.js https://nodejs.org/en/download/
  * OSX: Install Xcode
  * Windows: Install Python 2.7.3 https://www.python.org/
  * Open terminal (Mac) or powershell (Windows) `npm install -g node-gyp`
  * Follow the steps outlined in [Electron tasks Installation](https://github.com/Quobject/boscode-learn/blob/master/electron-tasks.md#installation)
  * Follow Hello World steps: https://github.com/rwaldron/johnny-five/wiki/Getting-Started#hello-world

___

## 01 Massimo Banzi: How Arduino is open-sourcing imagination 

Watch the video https://youtu.be/UoBUXOOdLXY and answer the following questions:

1. Massimo Banzi talks about a device powering the 3D printer. What is this device?  
2. Why did Massimo Banzi develop the Arduino?  
3. What are some projects that have been made using Arduino? List and describe 4 projects.  
4. Massimo Banzi states that Arduino is based on Open Source Hardware. Write up an overview of what Open Source Hardware is.  
5. Explain why it is possible for people to make their own Arduino boards.   
6. Visit the webpage Instructables http://www.instructables.com/ and pick a 'Technology' project you like and provide an overview of this project.  


___

## 02 Matt Richardson from Make gives an overview of the Arduino 

Watch the video https://youtu.be/CqrQmQqpHXc and answer the following questions:

1. Matt Richardson is from the Make Organisation. Please visit the Make site http://makezine.com/ and provide an overview of what Make is and what their purpose is. You may find it useful to read their 'About us' page located at the bottom-middle of their homepage.  
2. The Arduino is a micro-controller board. Provide a summary of Matt Richardson's overview of what a micro-controller board is.  
3. What is a Photo-Resistor and how could it be used?  
4. What is a Motion-Sensor and how could it be used?  
5. What is a GPS-Sensor and how could it be used?  
6. Provide an overview of the movie/lights out project Matt Richardson developed.  
7. The software provided by Arduino to program the Arduino board is free. Why is this the case?  

___

## 03 Arduino comic by Jody Culkin

http://bit.ly/1MOEAhk

Read each slide then answer the questions

1. Read slide 1. How does the slide describe an Arduino?  
2. Explain in your own words the following terms:Open Source, Electronics, Prototype, Platform  
3. Read slide 2. An Arduino contains a microchip. What is a microchip?  
4. Name two things that you can attach to the Arduino?  
5. Read slide  Give two examples of an Arduino Input.  
6. Give an example of an Arduino Output.  
7. Read slide 4. Define Voltage (V), and how is it measured.  
8. Define Current (I), and how is it measured.  
9. Define Resistance (R), and how is it measured.  
10. Explain what electricity is.  
11. As pictured, the water example is often used to explain V, I and R. In your own words explain the diagram. 
12. Read slide 5. OHM's law is based on the relationship between the Current (I), Resistance (R) and Voltage (V). Look at the water principle again to gain an understanding of OHM's law. So, lets think of OHM's law in regards to water flowing through a pipe. The Voltage (V) is the water pressure, the Current (I) is the amount of water flowing through the pipe, and the Resistance (R) is the size of the pipe. More water will flow through the pipe (current) the more pressure is applied (voltage) and the bigger the pipe is (lower the resistance). Once you have read the following web sites: http://bit.ly/1AlIJFA, http://bit.ly/1FuufVE, copy some of the formulas and underneath the formulas explain what they are doing.    
13. The slide shows a battery being used to light a lamp. What type of loop is being used?   
14. What is a schematic diagram?  
15. What happens when the switch in the schematic diagram is closed?  
16. Read slide 6. What is the difference between DC and AC?  
17. What do we attach the Ardunino to to i) Power it and ii) Program it?  
18. Read slide 7. What are the three Operating Systems Arduino can run on?  
19. Once the arduino is connected to a computer, how do you know it has power?  
20. In the software, you have to select the correct Arduino board you are using. This is done as pictured under the TOOLS tab. What type of board have they selected?  
21. Once you have selected your correct board (e.g. Arduino Uno), you must select the correct Serial Port. This is also done under the TOOLS tab. On a Mac, what type of serial port is selected?  
22. Read slide 8. What is an Integrated Development Environment (IDE)?  
23. A Sketch is another name for a program you have coded... Arduino has examples of sketchs (programs) in the IDE. Explain how you would open the Blink Sketch (program).  
24. How do you upload a sketch to the Arduino board?  
25. Read slide 9. As mentioned, a Sketch is basically a program of code that tells an Arduino how to act. The sketch has two main parts, what are they?  
26. Compare and contrast (explain the similarities and differences) between the Setup and Loop that are found in a sketch.  
27. A block of code is called a Function. How are Functions blocked out? Please insert the symbol used.  
28. The slide provides an example of code, please write next to the code below what it means.  
```
void setup (){
  pinmode(13, OUTPUT);
}
void loop ( ) {
  digitalWrite(13, HIGH);
  delay (1000); digitalWrite(13, LOW);
  delay (1000) ;
}
```
29. In the code above, the HIGH means Voltage is High and LOW means the voltage is LOW. If an LED Light was connected to pin 13, what would happen when the voltage was HIGH?  
30. Read slide 10. What is a breadboard and what is it used for?  
31. What does LED stand for?  
32. LED's can be placed in a breadboard. The LED has a longer and shorter leg. Please describe the names of each leg and what they are used for.  
33. Read slide 11. Looking at the code in the slide, in your own words, please explain what this code is doing, such as when it lights up an LED and when it does not.  
34. What is the difference between the Verify and Upload button in the Arduino IDE?  
35. Read slide 12. What is the switch used for?  
36. In the slide is some code using a switch. In your own words explain what the code is doing.  
37. Read slide 1 What does a POT stand for?  
38. What does a POT do?   
39. How can we view the range of values by turning the POT? HINT: It’s a feature in the IDE.     
40. Read slide 14. A new concept called "Variable' is added. What is a variable?    

___


## 04 Arduino Experimenter's Guide for NodeJS

* In terminal/powershell `cd c:\code\boscode-learn\code\arduino\01`.
* `npm install johnny-five`
* `git clone https://github.com/AnnaGerber/node-ardx.git && cd node-ardx`
* In visual studio code: File > Open Folder... `C:\code\boscode-learn\code\arduino\01\`.
* Setup circuit 1 http://node-ardx.org/exercises/1
* Run code examples from the terminal e.g. `node code/CIRC01-code-led-a-strobe.js`

Complete Exercises 1-14 at http://node-ardx.org/

For each exercise create the following documentation: 
  * Title  
  * Description  
  * Parts  
  * Circuit diagram  
  * Javascript code
  * Photo of your working circuit (showing clearly the St Luke's serial number of your assigned Arduino board)
  * Screen shot of the user interface (only if applicable)  

####Example

*Title* 01 Arduino Experimenter's Guide for NodeJS Exercise 1 Blinking LED  
*Description* LEDs (light emitting diodes) are used in all sorts of clever things which is why they are included in the Experimenter's kit. We will start off with something very simple, turning one on and off, repeatedly, producing a pleasant blinking effect.  
*Parts* 2 pin header x 4, 5mm LED, 330 ohm resistor (orange-orange-brown), jumper wires
*Circuit diagram*

 ![Circuit diagram]( images/001.jpeg "Circuit diagram") 
 
####Javascript code  
```
var five = require("johnny-five");
var myBoard, myLed;

myBoard = new five.Board();

myBoard.on("ready", function() {

  myLed = new five.Led(13);

  myLed.strobe( 1000 );

  // make myLED available as "led" in REPL

  this.repl.inject({
    led: myLed
  });

  // try "on", "off", "toggle", "strobe", "stop" (stops strobing)
});
```

####Photo

 ![Photo]( images/002.jpeg "Photo") 

####Screen shot



___

## 05 Arduino with Electron UI Getting Started

* Setup arduino board with one LED [as described here](http://node-ardx.org/exercises/1)
* If not done already, with your Arduino software upload `File > Examples > Firmata > StandardFirmataPlus`
* In your first terminal `cd c:\code\boscode-learn\code\arduino\02`.
* `npm install`
* `npm run server`
* Open a second terminal `cd c:\code\boscode-learn\code\arduino\02`.
* `npm run client`
* In visual studio code: File > Open Folder... `c:\code\boscode-learn\code\arduino\02`.
* Inspect files:
```bash
 client
   index.html
   main.js
   program.js
 server
   index.js
```
___

## 06 Arduino with Electron UI Button Pressing

* Setup arduino board with one LED and two buttons [as described here](http://node-ardx.org/exercises/7)
* If not done already, with your Arduino software upload `File > Examples > Firmata > StandardFirmataPlus`
* In your first terminal `cd c:\code\boscode-learn\code\arduino\03`.
* `npm install`
* `npm run server`
* Open a second terminal `cd c:\code\boscode-learn\code\arduino\03`.
* `npm run client`
* In visual studio code: File > Open Folder... `c:\code\boscode-learn\code\arduino\03`.
* Inspect files:
```bash
 client
   index.html
   main.js
   program.js
 server
   index.js
```
___

## 07 Arduino with Electron UI Twisting

* Setup arduino board with one LED and one potentiometer [as described here](http://node-ardx.org/exercises/8)
* If not done already, with your Arduino software upload `File > Examples > Firmata > StandardFirmataPlus`
* In your first terminal `cd c:\code\boscode-learn\code\arduino\04`.
* `npm install`
* `npm run server`
* Open a second terminal `cd c:\code\boscode-learn\code\arduino\04`.
* `npm run client`
* In visual studio code: File > Open Folder... `c:\code\boscode-learn\code\arduino\04`.
* Inspect files:
```bash
 client
   index.html
   main.js
   program.js
 server
   index.js
```
___


