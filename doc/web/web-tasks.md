# Web tasks

## Table of Content
    
[Installation]()  
[01 - Hello world]()  
[02 - Sequence]()  
[03 - Binary selection]()  
[04 - Multi way selection]()  
[05 - Pre-test loop]()  
[06 - Post-test loop]()  
[07 - Counted loop The challenge:]()  
[08 - Random numbers]()  
[09 - Change html]()  
[10 - Show image]()  
[11 - Button dropdowns]()  
[12 - Timer]()  
[13 - Array]()  
[14 - Record]()  
[15 - Array of Records]()  
___

## Installation

1. Create a github account: https://github.com/. Use your school email address and set username to stlukes-{first part of school email}. Sign into github.
2. In google chrome open cloud 9 https://c9.io/ and choose sign in with your github account.
3. In c9.io: Create a new workspace: 
  * Workspace name: web
  * Description: Learning javascript
  * Hosted workspace: Public
  * Clone from Git or Mercurial URL: `https://github.com/Quobject/boscode-web.git`
  * Choose a template: `Custom`
  * Hit 'Create workspace' button
4. Inside your workspace on the left side right click the folder name 'web' and select 'Open Terminal Here'
5. In your terminal type the command `npm install`  .
6. Type the command `grunt`.

  ```bash
  {yourname}:~/workspace (master) $ grunt
  Running "startServer" task
  Starting server ...OK

  Running "nodemon:dev" (nodemon) task
  [nodemon] 1.8.1
  [nodemon] to restart at any time, enter `rs`
  [nodemon] watching: *.*
  [nodemon] starting `node server.js`
  Your code is running at https://web-{yourname}.c9users.io
  ```

7. Open the url `https://web-{yourname}.c9users.io` in a new tab of Google Chrome.

___

## 01 - Hello world

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/01_Hello_world`.
2. Inside this folder inspect `index.html`:

  ```html
  <!DOCTYPE html>
  <html>
  <head>
      <title>01 - Hello world</title>
      <link rel="stylesheet" href="../third_party/bootstrap.min.css">
      <script src="../third_party/jquery.min.js"></script>
      <script src="../third_party/bootstrap.min.js"></script>
      <link rel="stylesheet" href="style.css">
      <script src="program.js"></script>
  </head>
  <body>
      <div class="container">
       

          <div class="row">
              <p>01 - Hello world</p>  
              <button id="runButton" type="button" class="btn btn-primary">Run</button>
          </div>
      </div>

  </body>
  </html>
  ```
  This file includes the usual bootstrap/jquery libraries. It also includes the `program.js` with the following content:

  ```js
  ﻿$(document).ready(function () {
    $("#runButton").click(program);
  });

  var program = function () {
    console.log("Hello world");
    console.log(5 + 6);

    var number1 = 5;
    var number2 = 6;
    var result = number1 + number2;
    console.log("The result is " + result);

  };
  ```

  The document ready event hooks up a click event handler for the button. Everytime a user clicks the function
  `program` executes.

3. Open `https://web-{yourname}.c9users.io/01_Hello_world/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to multiply 34 with 42


___

## 02 - Sequence

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/02_Sequence`.  
2. Inside this folder inspect `index.html`:

  ```html
  <!DOCTYPE html>
  <html>
  <head>
      <title>02 Sequence</title>
      <link rel="stylesheet" href="../third_party/bootstrap.min.css">
      <script src="../third_party/jquery.min.js"></script>
      <script src="../third_party/bootstrap.min.js"></script>
      <link rel="stylesheet" href="style.css">
      <script src="program.js"></script>
  </head>
  <body>

    <div class="container">
      <div class="row">
        <div class="input-group">
          <span class="input-group-addon" id="firstNumberLabel">First number</span>
          <input id="firstNumberInput" type="text" class="form-control" placeholder="First number" aria-describedby="firstNumberLabel" />
        </div>
        <div class="input-group">
          <span class="input-group-addon" id="secondNumberLabel">Second number</span>
          <input id="secondNumberInput" type="text" class="form-control" placeholder="Second number" aria-describedby="secondNumberLabel" />
        </div>
        <button id="runButton" type="button" class="btn btn-primary">Run</button>
      </div>
    </div>

  </body>
  </html>
  ```
  This file includes the usual bootstrap/jquery libraries. It also includes the `program.js` with the following content:

  ```js
  $(document).ready(function () {
    $("#runButton").click(add2Numbers);
  });

  var add2Numbers = function () {
    var firstNumber = $("#firstNumberInput").val();
    firstNumber = parseInt(firstNumber);

    var secondNumber = $("#secondNumberInput").val();
    secondNumber = parseInt(secondNumber);

    var total = firstNumber + secondNumber;

    console.log("the sum of your 2 numbers is " + total);
  };
  ```

  The document ready event hooks up a click event handler for the button. Everytime a user clicks the function
  `program` executes.

3. Open `https://web-{yourname}.c9users.io/02_Sequence/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.  
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to multiply both numbers.


___

## 03 - Binary selection

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/03_Binary_selection`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/03_Binary_selection/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to to ask for the age. If the age is above 18 display "You can vote."



___

## 04 - Multi way selection

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/04_Multi-way_selection`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/04_Multi-way_selection/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Write a set of instructions that translates a dice integer into the corresponding word. Modify program.js: set a variable dice to an integer e.g. 1 and then use a multiway selection to display the word e.g. "one". If the integer is not between 1 and 6 display "invalid dice value".   


___

## 05 - Pre-test loop

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/05_Pre-test_loop`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/05_Pre-test_loop/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to display the even numbers from 2 to 20.   


___

## 06 - Post-test loop

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/06_Post-test_loop`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/06_Post-test_loop/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to display the the odd numbers from 23 to 33.   



___

## 07 - Counted loop

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/07_Counted_loop`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/07_Counted_loop/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to print out the 7 times table. 


___

## 08 - Random numbers

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/08_Random_numbers`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/08_Random_numbers/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to print a random number between 1 and 100.



___

## 09 - Change html

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/09_Change_html`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/09_Change_html/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to display a counter 1, 2 ... on the website with every press of Run.


___

## 10 - Show image

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/10_Show_image`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/10_Show_image/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js` to display random images of a dice with 1 - 6 dots.


___

## 11 - Button dropdowns

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/11_Button_dropdowns`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/11_Button_dropdowns/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `index.html` to add more options.



___

## 12 - Timer

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/12_Timer`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/12_Timer/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js`: Change the start time of the timer.


___

## 13 - Array

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/13_Array`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/13_Array/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js`: Add another name to the array.



___

## 14 - Record

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/14_Record`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/14_Record/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js`: Create another product record with: id = 2, name = Dishwasher Tablets, description = ... and add the description to the console log statement.


___

## 15 - Array of Records

1. In your cloud 9 workspace `web` open the folder `/home/ubuntu/workspace/public/15_Array_of_records`.
2. Inside this folder inspect `index.html` and `program.js`.   
3. Open `https://web-{yourname}.c9users.io/15_Array_of_records/` in Google Chrome  and also open the developer tools: Windows: `F12` or `Ctrl-shift+I`, Mac: `Cmd + Opt + I`.
4. Click the button and observe the console output.

###### The challenge:

Modify `program.js`: Add a third product and include the description in the print out.





