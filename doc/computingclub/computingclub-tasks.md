# Computingclub tasks

## Table of Content
    
[Installation](#installation)  
[01 - Hello world](#01---hello-world)  

___

## Installation

Follow steps at https://github.com/Quobject/boscode-learn#installation


## Tasks

### 01 Using a variable

JavaScript variables are containers for storing data values. Read information at http://www.w3schools.com/js/js_variables.asp

```js
//Using a variable
var boscode = require('boscode');

var score;
score = 100;
boscode.display(score);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/01/app.js` by double clicking it in the file tree.
2. Right click the file `app.js` and choose `Open Terminal Here`.
3. In your bash terminal type `ll` to see the content of the current directory. Type `pwd` to see the working directory, verify that this is  `/home/ubuntu/workspace/code/computingclub/01/app.js`.
4. Type `node app.js` to run the program.
5. Change the value assigned to score. Run the program again.
6. Declare a second variable, maybe score2.
7. Assign your variable a value.
8. Use boscode.display to display your variable.
9. Paste your completed code into your google docs solution document.



### 02 Variables vary

JavaScript syntax is the set of rules, how JavaScript programs are constructed. Read information at http://www.w3schools.com/js/js_syntax.asp


```js
//Variables vary
var boscode = require('boscode');


var score;
score = 100;
boscode.display(score);

score = 150;
boscode.display(score);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/02/app.js` by double clicking it in the file tree.
2. Right click the file `app.js` and choose `Open Terminal Here`.
3. In your bash terminal type `ll` to see the content of the current directory. Type `pwd` to see the working directory, verify that this is  `/home/ubuntu/workspace/code/computingclub/02/app.js`.
4. Type `node app.js` to run the program.
5. Change the value assigned to score. Run the program again.
6. Declare a second variable, maybe score2.
7. Assign your variable a value.
8. Use boscode.display to display your variable on the console.
9. Can you display the sum of the two variables?
10. Paste your completed code into your google docs solution document.



### 03 Assigning text to variables
JavaScript strings are used for storing and manipulating text. Read information at http://www.w3schools.com/js/js_strings.asp

```js
//Assigning text to variables
var boscode = require('boscode');

var message;

message = "Hello World!";
boscode.display(message);

message = 'Congratulations! Your tweet has won a prize...';
boscode.display(message);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/03/app.js` by double clicking it in the file tree.
2. Right click the file `app.js` and choose `Open Terminal Here`.
3. In your bash terminal type `ll` to see the content of the current directory. Type `pwd` to see the working directory, verify that this is  `/home/ubuntu/workspace/code/computingclub/03/app.js`.
4. Type `node app.js` to run the program.
5. Assign message a third value. Display it on the console.
6. Pieces of text can be joined together using the + symbol.  e.g. `"Hello " + "World!"`
7. Split the first message into two pieces, joined by + and run the program.
8. Split the second message into three pieces, joined by + and run the program. Be careful to use matching speech marks.
9. Paste your completed code into your google docs solution document.


### 04 Declaring and assigning in two steps

Assignment operators assign values to JavaScript variables. Read information at http://www.w3schools.com/js/js_assignment.asp

```js
//Declaring and assigning in two steps
var boscode = require('boscode');

var playerName;
var locationName;

playerName = "Kandra";
locationName = "The Dungeon of Doom";

boscode.display(playerName + " is in " + locationName);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/04/app.js` by double clicking it in the file tree.
2. Right click the file `app.js` and choose `Open Terminal Here`.
3. In your bash terminal type `ll` to see the content of the current directory. Type `pwd` to see the working directory, verify that this is  `/home/ubuntu/workspace/code/computingclub/04/app.js`.
4. Type `node app.js` to run the program.
5. Declare a score variable.
6. Assign it a value.
7. Display an extra message on the console, by combining variables and strings, to say something like "Kandra has a score of 100".
8. Paste your completed code into your google docs solution document.



### 05 Declaring and assigning in one step

JavaScript statements are "instructions". Read information at http://www.w3schools.com/js/js_statements.asp

```js
//Declaring and assigning in one step
var boscode = require('boscode');

var playerName = "Kandra";
var locationName = "The Dungeon of Doom";

boscode.display(playerName + " is in " + locationName);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/05/app.js` by double clicking it in the file tree.
2. Right click the file `app.js` and choose `Open Terminal Here`.
3. In your bash terminal type `ll` to see the content of the current directory. Type `pwd` to see the working directory, verify that this is  `/home/ubuntu/workspace/code/computingclub/05/app.js`.
4. Type `node app.js` to run the program.
5. Declare a health variable and assign it a value in one step.
6. Declare a message variable.
7. Assign message a value created by joining variables and text to say something like "Kandra has health 50 and is in The Dungeon of Doom".
8. Replace the current boscode.display statement with a new one to display the message variable.
9. Paste your completed code into your google docs solution document.


### 06 Using a variable’s current value to set its new value

Arithmetic operators are used to perform arithmetic on numbers (literals or variables). Read information at http://www.w3schools.com/js/js_operators.asp

```js
//Using a variable’s current value to set its new value
var boscode = require('boscode');

var score;

score = 100;
boscode.display("Your score was " + score);

boscode.display("Great splat!!!");
score = score + 50;
boscode.display("New score: " + score);

boscode.display("Way to go!");
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/06/app.js`.
2. Run the program.
3. Add 100 to the player's score
4. Show the new score.
5. Display a message of congratulations.
6. Paste your completed code into your google docs solution document.


### 07 Valid and invalid variable names


```js
//Valid and invalid variable names

var thisIsFine;
var $noProblemHere;
var _underscore56;
var StartWithCapital;
var z5;

var 999;
var 39Steps;
var &nope;
var single words only;
var yield; 
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/07/app.js`.
2. Take a look at the errors in the cloud 9 editor.
3. Run the program and see what errors appear.
4. Delete the second block of variables one by one from the code. See how the errors change.
5. Paste your completed code into your google docs solution document.




continue: https://github.com/jrlarsen/GetProgramming/blob/master/Chapter_03_Objects/chapter3.md


### 08


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/08/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 09


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/09/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 10


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/10/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 11


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/11/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 12


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/12/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 13


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/13/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 14


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/14/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 15


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/15/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 16


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/16/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 17


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/17/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 18


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/18/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.





### 19


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/19/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 20


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/20/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.





### 21


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/21/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 22


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/22/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.






### 23


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/23/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.





### 24


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/24/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.







### 25


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/25/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.







### 26


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/26/app.js`.
2. Run the program.
5. 
9. Paste your completed code into your google docs solution document.





