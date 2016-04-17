# Computingclub tasks

## Table of Content
    
[Installation](#installation)  
[01 - Hello world](#01---hello-world)  

___

## Installation

Follow steps at https://github.com/Quobject/boscode-learn#installation


## Tasks

### 01 Using a variable

What is a variable?

A variable is a named value in our program. Whenever you use the name in the program, it is replaced with the value. You could create a variable called score and give it the value 100. Then, if you tell the computer to “display the score,” it will display 100. Now, variables can change, hence the name, so later in the program, maybe in response to some action a player takes, you can update the score. If you add 50 to score and tell the computer to “display the score,” it will now display 150.


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

Declaring variables and assigning values

Letting the computer know about information you’d like to store requires two steps:

1. you need to set a name you can use to refer to your data in the program, like score or playerName or taxRate, and

2. you need to link the name with the value you want to store. Something like set score equal to 100 or make ‘George’ the playerName or let the tax rate be 12%.


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

Programmers call sections of text strings because they are strings, or sequences, of characters. To denote a string you place the text inside of quotation marks. The marks can be double, "Hello World!", or single, 'Congratulations!', as long as they match. Without the quotation marks, JavaScript would try to interpret the text as instructions or variables.

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

You have seen how to declare variables and then assign them values in two steps. It’s also possible to declare a variable and assign it a value in a single statement.


If you know the value of a variable at the time you declare it, then this single step approach can be a neat way of assigning the value to the variable. Sometimes, the value won’t be known at the time of declaration; maybe some calculations need to be performed, user input is required or you’re waiting for a network response. In that case, declaration and assignment would be separate. It is common for programmers to declare their variables at the top of a program, even if they won’t assign them values until later.


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


When you assign a value to a variable, JavaScript evaluates the expression to the right of the assignment operator and assigns the result to the variable.

```js
var score;

score = 100 + 50;
```


JavaScript evaluates the expression, 100 + 50, and assigns the result, 150, to the variable score.

The values in the expression probably won’t be hard-coded literals like 100 and 50; they’re more likely to be variables. Here’s an example, using the variables callOutCharge, costPerHour and numberOfHours, to calculate the total cost when hiring a plumber to do some work:

```
total = callOutCharge + costPerHour * numberOfHours;
```


The * symbol is used for multiplication; it is the multiplication operator. You can also use – for subtraction and / for division.

Because JavaScript evaluates the expression on the right first, before assigning its value to the variable on the left, you can even use the current value of a variable to set its new value. Say a player in your app sensation The Fruitinator! has just splatted a strawberry; that’s 50 points! The player needs an update.


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


#### Choosing good variable names

In all the code listings so far, there was nothing forcing you to give the variables the names you did. You tried to choose names that would help anyone reading the code understand the purpose of the variables. You almost have a free choice but must be careful not to tread on JavaScript’s toes; there are names that JavaScript has set aside for its own use and some further rules governing valid variable names.

#### Keywords and reserved words

JavaScript has a set of keywords, like var and function, that are part of the language itself and govern the actions and properties available in every program. It also sets aside some reserved words that may turn up as keywords in the language in the future. You can’t use those keywords or reserved words as variable names. Other examples of keywords are if, switch, do and yield and a full list can be found on the Mozilla Developer Network. 


You don’t have to learn the lists of keywords and reserved words; you’ll pick up most of them as you do more programming and they usually throw errors when you try to use them. However, do bear them in mind if your program is not working and you’re not sure why.

#### Rules for naming variables

So now that keywords and reserved words are out, is everything else in? Not quite - there are a few further rules. Variable names can start with any letter, a dollar sign, $, or an underscore, _. Subsequent characters can be any of those, or numbers. Spaces are not allowed. 


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


### 08 A book as an object


Sometimes it makes sense to group items together and see them as a whole. Consider a first aid kit: we happily treat it as a single item – “Have you packed the first aid kit?” “Pass the first aid kit,” “We need the first aid kit, NOW!” – but will quickly switch focus to its contents when the need arises – “Pass the antiseptic and the bandages from the first aid kit, please.” A number of items is neatly encapsulated by a single object.

JavaScript objects  are a simple and efficient way to collect variables together so that you can pass them around as a group rather than individually.


```
var book;

book = {
    title : "The Hobbit",
    author : "J. R. R. Tolkien",
    published : 1937
};

console.log(book);
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





