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

boscode.display(book);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/08/app.js`.    
2. Run the program.  
3. Change the title of book to "The Hobbit, or There and Back Again".  
4. Run the program again.  
5. Try creating a book2 object.  
6. Display book2 to the console.  
7. Paste your completed code into your google docs solution document.  




### 09 Using dot notation to access property values

For JavaScript objects, to access the values of an object’s properties you can use dot notation. Join the name of the variable to the name of the property, its key, with a period or dot. For a first aid kit as an object you might use kit.antiseptic or kit.scissors or kit.bandages. And for books, to access the author property of the object assigned to the variable called book, you write book.author.


```js
var book;

book = {
    title : "The Hobbit",
    author : "J. R. R. Tolkien",
    published : 1937
};

boscode.display(book.title);
boscode.display(book.author);
```



###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/09/app.js`.
2. Run the program.
3. Log the published property to the console.  
4. Add a second book.  
5. Display its details to the console.  
6. Paste your completed code into your google docs solution document.  



### 10 Concatenating string properties

Replacing a bunch of separate variables with a single object helps you manage the complexity of your programs. You can think more clearly about how programs work when details are hidden until you need them. You consider a book a single entity in your program until you need to access the book’s title or author or publication date. It may seem that replacing three variables with one variable and three properties isn’t an improvement but when you start to use objects with functions and arrays, their economy and clarity will be more obvious.

You use property values just like variables. The code below concatenates each book’s title with the string " by " and its author to give:

```bash
The Hobbit by J. R. R. Tolkien
Northern Lights by Philip Pullman
```


```js
//Concatenating string properties
var boscode = require('boscode');

var book1;
var book2;

book1 = {
  title: 'The Hobbit',
  author: 'J. R. R. Tolkien'
};

book2 = {
  title: 'Northern Lights',
  author: 'Philip Pullman'
};

boscode.display(book1.title + ' by ' + book1.author);
boscode.display(book2.title + ' by ' + book2.author);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/10/app.js`.   
2. Run the program.  
3. Add a third book.  
4. Log its details to the console.   
5. Add a third property.  
6. Update the messages displayed to include the new property.  
7. Paste your completed code into your google docs solution document.  



### 11 Using dot notation to update a property

In a quiz app, players attempt questions one after another. The number of questions attempted, number of questions correct and score will change over time. You can create a player object with initial values set and then update them whenever a question is attempted. Use dot notation to change a property that already exists or to add a new property to an object.


Your code below sets the `attempted` and `correct` properties to an initial value when the object is created but then updates them to a new value. It uses the assignment operator, =, to assign the value, 1, on the right of the operator, to the property, `player1.attempted`, on its left. You set the `attempted` and `correct` properties and then immediately update them; in the actual quiz app, the change would be in response to the player answering a question.

You can add new properties to an object after creating it. You assign the value 50 to the score property of the player1 object.  

```js
player1.score = 50;
```

You didn’t set the score property when creating the object; assigning a value automatically creates the property if it does not yet exist.  


```js
var boscode = require('boscode');

var player1;

player1 = {
  name: "Max",
  attempted: 0,
  correct: 0
};

player1.attempted = 1;
player1.correct = 1;
player1.score = 50;

boscode.display('player1 = ', player1);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/11/app.js`.
2. Run the program.
3. Change the value of the score property by typing `player1.score = 100;`.
4. Update other properties.
5. Paste your completed code into your google docs solution document.


### 12 Using a property in a calculation

Just like variables, you can use properties in a calculation and assign the result back to the property. Listing below shows code updating a player’s properties.  

```bash
> Max has scored 0
> Max has scored 50
```

When you update the score property, JavaScript evaluates the right hand side of the assignment first. As player1.score is 0, the expression becomes 0 + 50 which is 50. JavaScript then assigns that value to the left hand side, i.e. back to the score property. So, you update player1.score from 0 to 50.  

```js
var boscode = require('boscode');

var player1;

player1 = {
  name: 'Max',
  score: 0
};

boscode.display(player1.name + ' has scored ' + player1.score);

player1.score = player1.score + 50;

boscode.display(player1.name + ' has scored ' + player1.score);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/12/app.js`.
2. Run the program.
3. Write code to increase player1's score by 10%.
4. Add a second player.
5. Use the players' properties to find the sum of their scores and display it to the console, along with an appropriate message that includes their names.
6. Paste your completed code into your google docs solution document.


### 13 A blog post

A blog is made up of blog posts. It would be good to have more information about each author, to be able to tag posts with keywords and to add comments to each post. For now, here’s a minimal object to represent a single post.

```js
var boscode = require('boscode');

var post = {
  id: 1,
  title: 'My Crazy Space Adventure',
  author: 'Philae',
  created: '2015-06-21',
  approved: true,
  body: 'You will not believe where I just woke up!! Only on a comet...'
};

boscode.display('post = ', post);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/13/app.js`.
2. Run the program.
3. Add a second post. 
4. Display the second post to the console.
5. Paste your completed code into your google docs solution document.


### 14 A calendar event

Calendar events clearly involve dates. JavaScript does have a Date object but you won’t be using it. Listing below represents dates as strings in a specific format.  

Include an apostrophe in the string when the string is delimited by double quotes.  
 
Use an escaped apostrophe when the string is delimited by single quotes.  

Notice how to cope with the apostrophe in the notes property. A backslash character before the apostrophe stops JavaScript from seeing it as the end of the string. The backslash is called an escape character and won’t be shown.  

```js
event.notes = 'Don\'t forget the portfolio!';
```

Use the escape character to display double quotes when a string is already wrapped in double quotes.
```js
var story = "She looked at me. \"What did you say?\" she asked.";
```



```js
var boscode = require('boscode');


var event = {
  title: "Appraisal Meeting",
  startDate: "2016-10-04 16:00:00",
  endDate: "2016-10-04 17:00:00",
  location: "Martha's office",
  importance: 1,
  notes: 'Don\'t forget the portfolio!'
};

boscode.display('event = ', event);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/14/app.js`.  
2. Run the program.  
3. Remove the backslash from the notes property.  
4. Take a look at the errors reported.  
5. Put the backslash back.  
6. See how the location property doesn't need a backslash. What happens if you add one and log the location property?  
7. What if you want to show a backslash as part of a string?  
8. Paste your completed code into your google docs solution document.  



### 15 A question and answer for a quiz app

A quiz app is likely to include a small set of question types. Listing below is an example of a multiple choice question type. Each type of question would have a fixed form of presentation. 

```js
var boscode = require('boscode');


var questionAndAnswer = {
  question: 'What is the capital of France?',
  answer1: 'Bordeaux',
  answer2: 'F',
  answer3: 'Paris',
  answer4: 'Brussels',
  correctAnswer: 'Paris',
  marksForQuestion: 2
};

boscode.display('questionAndAnswer = ', questionAndAnswer);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/15/app.js`.
2. Run the program.
3. Use boscode.display to present the question and answer options in a nicely formatted way.
4. Paste your completed code into your google docs solution document.


### 16 A player object

Clearly, it’s much neater to use JavaScript objects as a way of grouping together all of the information about a single player. Listing below shows how you can represent a player as an object and display some of their properties on the console. The output is:

```bash
> Kandra
> Kandra is in The Dungeon of Doom
> Kandra has health 50
> Items: a rusty key, The Sword of Destiny, a piece of cheese
```

The last four lines of the listing are just for displaying player information. Having to repeat those lines of code every time you want to display a player’s information seems a little tedious. It would be great to be able to write the lines of code once and then call them up on demand.

You’re in luck! JavaScript lets you define functions to execute blocks of code whenever you need them. Functions are very powerful and will help streamline the display of player properties and the creation of multiple player objects.

```js
var boscode = require('boscode');

var player;

player = {
  name: 'Kandra',
  health: 50,
  place: 'The Dungeon of Doom',
  items: 'a rusty key, The Sword of Destiny, a piece of cheese'
};

boscode.display(player.name);
boscode.display(player.name + ' is in ' + player.place);
boscode.display(player.name + ' has health ' + player.health);
boscode.display('Items: ' + player.items);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/16/app.js`.
2. Run the program.  
3. Create a second player.  
4. Log their details to the console.  
5. Paste your completed code into your google docs solution document.  

Notice how storing the items as a string isn't a great approach. If the player drops an item we'll have to manipulate the string to remove the item. JavaScript has a way of storing lists of items called an array. 


###### Summary Objects

- Group related variables together as properties of an object.  
- Define objects as collections of comma separated properties between curly braces.  

```
var player = { name : "Hadfield", location : "The ISS" };
```

- For each property use a key-value pair, with key and value separated by a colon.  

```
name : "Hadfield"
```

- Access property values by using dot notation. If the object is assigned to a variable, join the property name to the variable name with a dot.  

```
player.name
```

- Use properties in expressions just as you would variables.

```
console.log(player.name + " is in " + player.location);
```

- Assign values to properties using the assignment operator, =.

```
player.location = "On a space walk";
```

- Add new properties to existing objects whenever you want.

```
player.oxygen = 96;
```


### 17


* Organizing instructions with functions  
* Defining a function – specifying code to be executed on demand  
* Calling a function – executing code on demand  
* Reducing repetition in code  
* Making programs easier to read and update  

One of the main themes of of JavaScript is managing complexity through good organization. You stored information in variables and saw how choosing good names for those variables helps you understand their purpose in a program. Then you grouped variables together as properties of objects. You can focus on objects as a whole or drill down into the details when needed. Now you take a look at another important method for organizing code and avoiding repetition, the function.

* Noticing repetition

As the programs you write become longer and more complex, you find yourself repeating similar sections of code with only slight differences. There are common tasks, like displaying text, animating an image or saving to a database, that may need to be performed often. You need to notice these recurring bits of code; they are prime function fodder.

A function is a way of writing code once but using it many times. Section 4.2 looks at how to create functions. This section explores a couple of examples of JavaScript repeated.


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





