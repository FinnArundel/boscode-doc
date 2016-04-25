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


### 17 Displaying an object's properties on the console


* Organizing instructions with functions  
* Defining a function – specifying code to be executed on demand  
* Calling a function – executing code on demand  
* Reducing repetition in code  
* Making programs easier to read and update  

One of the main themes of of JavaScript is managing complexity through good organization. You stored information in variables and saw how choosing good names for those variables helps you understand their purpose in a program. Then you grouped variables together as properties of objects. You can focus on objects as a whole or drill down into the details when needed. Now you take a look at another important method for organizing code and avoiding repetition, the function.

* Noticing repetition

As the programs you write become longer and more complex, you find yourself repeating similar sections of code with only slight differences. There are common tasks, like displaying text, animating an image or saving to a database, that may need to be performed often. You need to notice these recurring bits of code; they are prime function fodder.

A function is a way of writing code once but using it many times. This section explores a couple of examples of JavaScript repeated.


```js
var boscode = require('boscode');

var movie1;

movie1 = {
  title: 'Inside Out',
  actors: 'Amy Poehler, Bill Hader',
  directors: 'Pete Doctor, Ronaldo Del Carmen'
};

boscode.display('Movie information for ' + movie1.title);
boscode.display('------------------------------');
boscode.display('Actors: ' + movie1.actors);
boscode.display('Directors: ' + movie1.directors);
boscode.display('------------------------------');
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/17/app.js`.
2. Run the program.
3. Add a second movie and display the same info for it.
4. Create an object to represent a blog post.
5. Write code to display info about the blog post.
6. Paste your completed code into your google docs solution document.


### 18 Displaying information from similar objects

If you have to write those five lines of code every time you want to display movie information and for every movie, that’s going to get pretty repetitive. And if you then decide to change the information displayed, you’ll have to go through all the places where it appears in the code and make sure it’s changed consistently.

The next listing shows the code repeated for three different movies.


```js
var boscode = require('boscode');

var movie1;
var movie2;
var movie3;

movie1 = {
  title: 'Inside Out',
  actors: 'Amy Poehler, Bill Hader',
  directors: 'Pete Doctor, Ronaldo Del Carmen'
};

movie2 = {
  title: 'Spectre',
  actors: 'Daniel Craig, Christoph Waltz',
  directors: 'Sam Mendes'
};

movie3 = {
  title: 'Star Wars: Episode VII - The Force Awakens',
  actors: 'Harrison Ford, Mark Hamill, Carrie Fisher',
  directors: 'J.J.Abrams'
};

boscode.display('Movie information for ' + movie1.title);
boscode.display('------------------------------');
boscode.display('Actors: ' + movie1.actors);
boscode.display('Directors: ' + movie1.directors);
boscode.display('------------------------------');

boscode.display('Movie information for ' + movie2.title);
boscode.display('------------------------------');
boscode.display('Actors: ' + movie2.actors);
boscode.display('Directors: ' + movie2.directors);
boscode.display('------------------------------');

boscode.display('Movie information for ' + movie3.title);
boscode.display('------------------------------');
boscode.display('Actors: ' + movie3.actors);
boscode.display('Directors: ' + movie3.directors);
boscode.display('------------------------------');
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/18/app.js`.
2. Run the program.  
3. Add a fourth movie and display its info.  
4. All the movie info is in one big block on the console.  Change the code to space out the different movies.  
5. Create objects to represent three calendar events.  
6. Display info from the three events on the console.  
7. Paste your completed code into your google docs solution document.  






### 19 Adding tax to find the total cost

A simple task like adding tax to a price is the kind of thing that happens again and again. You calculate the tax and add it to the price to give a total cost.  

```bash
> price = $140
> tax @ 15% = $21
> total cost = $161
```


```js
var boscode = require('boscode');

var sale1;
var sale2;
var sale3;

sale1 = { price: 140, taxRate: 15 };
sale2 = { price: 40, taxRate: 10 };
sale3 = { price: 120, taxRate: 20 };

sale1.tax = sale1.price * sale1.taxRate / 100;
sale2.tax = sale2.price * sale2.taxRate / 100;
sale3.tax = sale3.price * sale3.taxRate / 100;

sale1.total = sale1.price + sale1.tax;
sale2.total = sale2.price + sale2.tax;
sale3.total = sale3.price + sale3.tax;

boscode.display('price = $' + sale1.price);
boscode.display('tax @ ' + sale1.taxRate + '% = $' + sale1.tax);
boscode.display('total cost = $' + sale1.total);

boscode.display('price = $' + sale2.price);
boscode.display('tax @ ' + sale2.taxRate + '% = $' + sale2.tax);
boscode.display('total cost = $' + sale2.total);

boscode.display('price = $' + sale3.price);
boscode.display('tax @ ' + sale3.taxRate + '% = $' + sale3.tax);
boscode.display('total cost = $' + sale3.total);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/19/app.js`.
2. Run the program.
3. Add the details for a fourth sale.  
4. Display the fourth sale to the console. Use the same format as the others.
5. Add code to separate out the different sales on the console.  
6. Paste your completed code into your google docs solution document.



### 20 A simple function definition and assignment

Just as an object is a collection of properties, a function is a collection of statements or instructions. Functions help you avoid repetition and make your code more organized and easier to update and maintain. Well-named functions should also make your programs easier to follow. If you find your functions are used a lot in a program and would be useful in other programs too, you can even create libraries of helpful functions to include in other projects.

In the previous section you saw two examples of programs where blocks of code with the same structure were repeated. To reduce the code bloat you want to replace those blocks with something like the following:

```js
showMovieInfo();

showCostBreakdown();
```


The two functions, showMovieInfo and showCostBreakdown should produce the same output as the code blocks in tasks 18 & 19, and you should be able to use them again and again, whenever you want. Let’s see how such code on demand magic is conjured.

#### Defining new functions

Define a function by using:

- the function keyword,  
- parentheses, (), and  
- a code block between curly braces, {}.  

The code block contains the list of instructions you would like to execute whenever you use the function. The list of instructions is also called the function body.  

It is common to see function definitions set out like this:

```js
function () {

// lines of code to be executed go here

}
```

Once you have defined a function, you can assign it to a variable, just like any value. Listing below defines a function to display “Hello World!” on the console and assigns the function to the variable sayHello.


```js
var boscode = require('boscode');

var sayHello;

sayHello = function () {
  boscode.display('Hello World!');
};

sayHello();
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/20/app.js`.
2. Run the program.
3. Add a second sayHello(); on a new line. Run the program.
4. Change the message from the sayHello function.
5. Create a sayGoodbye function.
6. Make the program say goodbye ten times.
7. Paste your completed code into your google docs solution document.


### 21 Two more function definitions and assignments


```js
var boscode = require('boscode');

var findTotal;
var displayMenu;

findTotal = function () {
  result = number1 + number2;
};

displayMenu = function () {
  boscode.display('Please choose an option:');
  boscode.display('(1) Print log');
  boscode.display('(2) Upload file');
  boscode.display('(9) Quit');
};
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/21/app.js`.
2. Run the program.  
3. Declare number1, number2 and result variables.   
4. Assign values to the number1 and number2 variables.  
5. Run the findTotal function by writing its name followed by parentheses: findTotal();
6. Display the result on the console.
7. Run the displayMenu function. 
9. Paste your completed code into your google docs solution document.


### 22 Calling the sayHello function three times

Once you have assigned a function to a variable, whenever you want to execute the statements in the function body, you write the variable name followed by parentheses, ().

```js
sayHello();

findTotal();

displayMenu();
```

Other names for running the function are calling the function or invoking the function.

In listing below, you call the sayHello function three times. It displays the string “Hello World!” three times, like this:

```bash
> Hello World!
> Hello World!
> Hello World!
```

```js
var boscode = require('boscode');

var sayHello;

sayHello = function () {
  boscode.display('Hello World!');
};

sayHello();
sayHello();
sayHello();
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/22/app.js`.  
2. Run the program.  
3. Change the message from the sayHello function.  
   To add a line-break to a string, insert '\n'    
   e.g. "Line One\nLine Two"    
4. Break the Hello World! message across two lines.    
5. Create a function that prints the letters of "Hello World!" one by one down the page.  
6. Paste your completed code into your google docs solution document.  



### 23 Using the findTotal function to display a calculation


Listing below uses the findTotal function to update the result variable. It then displays the whole calculation on the console:

```
> 1000 + 66 = 1066
```


```js
var boscode = require('boscode');

var number1 = 1000;
var number2 = 66;
var result;
var findTotal;

findTotal = function () {
  result = number1 + number2;
};

findTotal();

boscode.display(number1 + ' + ' + number2 + ' = ' + result);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/23/app.js`.
2. Run the program.
3. Change number1 and number2 and run the program.  
4. Add a third variable, number3, and assign it a value.
5. Update the findTotal function to add the three numbers.  
6. Update the boscode.display line to show the new calculation.
7. Paste your completed code into your google docs solution document.



### 24 Using a function to display object properties


The code below assigns the new function to the showMovieInfo variable. Call the function by writing the variable name followed by parentheses, showMovieInfo(), as seen in the next listing. You should end up with the following output on the console.

```bash
> Movie information for Inside Out
> ------------------------------
> Actors: Amy Poehler, Bill Hader
> Directors: Pete Doctor, Ronaldo Del Carmen
> ------------------------------
```


```js
var boscode = require('boscode');

var showMovieInfo;

showMovieInfo = function () {
  boscode.display('Movie information for ' + movie.title);
  boscode.display('------------------------------');
  boscode.display('Actors: ' + movie.actors);
  boscode.display('Directors: ' + movie.directors);
  boscode.display('------------------------------');
};

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/24/app.js`.  
2. Run the program.  
3. Add a call to showMovieInfo and run the program. What happens?  
4. Declare a movie variable but don't assign it a value. Run the program. What happens now?  
5. Create an empty object and assign it to the movie variable. Run the program again. Does the output change?  
6. Add title, actors and directors properties to the movie object. Run one more time. Is the output as expected?  
7. Paste your completed code into your google docs solution document.


### 25 Calling the showMovieInfo function


```js
var boscode = require('boscode');

var movie1;
var showMovieInfo;
var movie;

movie1 = {
  title: 'Inside Out',
  actors: 'Amy Poehler, Bill Hader',
  directors: 'Pete Doctor, Ronaldo Del Carmen'
};

showMovieInfo = function () {
  boscode.display('Movie information for ' + movie.title);
  boscode.display('------------------------------');
  boscode.display('Actors: ' + movie.actors);
  boscode.display('Directors: ' + movie.directors);
  boscode.display('------------------------------');
};

movie = movie1;

showMovieInfo();
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/25/app.js`.
2. Run the program.
3. Without declaring a movie2 variable, assign movie2 to the movie variable instead of movie1. i.e. movie = movie2; What happens when you call showMovieInfo?
4. Create an empty object and assign it to a movie2 variable. What happens when you call showMovieInfo now?
5. Fill out movie2 with the properties needed by showMovieInfo. What happens when you call showMovieInfo now?
6. Paste your completed code into your google docs solution document.


### 26 Using the same function with multiple objects


```js
//Using the same function with multiple objects
var boscode = require('boscode');

var movie1;
var movie2;
var movie3;
var movie;
var showMovieInfo;

movie1 = {
  title: 'Inside Out',
  actors: 'Amy Poehler, Bill Hader',
  directors: 'Pete Doctor, Ronaldo Del Carmen'
};

movie2 = {
  title: 'Spectre',
  actors: 'Daniel Craig, Christoph Waltz',
  directors: 'Sam Mendes'
};

movie3 = {
  title: 'Star Wars: Episode VII - The Force Awakens',
  actors: 'Harrison Ford, Mark Hamill, Carrie Fisher',
  directors: 'J.J.Abrams'
};

showMovieInfo = function () {
  boscode.display('Movie information for ' + movie.title);
  boscode.display('------------------------------');
  boscode.display('Actors: ' + movie.actors);
  boscode.display('Directors: ' + movie.directors);
  boscode.display('------------------------------');
};

movie = movie1;
showMovieInfo();

movie = movie2;
showMovieInfo();

movie = movie3;
showMovieInfo();


```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/26/app.js`.
2. Run the program.
3. Create an object to represent a multiple choice quiz question.  
4. Create two more quiz question objects.  
5. Create a function to show the question and answer options.  
6. Use the same variable assignment technique as above to display all three questions on the console.  
7. Paste your completed code into your google docs solution document.



### 27 Using functions to add and display tax


```js
var boscode = require('boscode');

var sale1;
var sale2;
var sale3;
var sale;
var calculateTax;
var displaySale;

sale1 = { price: 140, taxRate: 15 };
sale2 = { price: 40, taxRate: 10 };
sale3 = { price: 120, taxRate: 20 };

calculateTax = function () {
  sale.tax = sale.price * sale.taxRate / 100;
  sale.total = sale.price + sale.tax;
};

displaySale = function () {
  boscode.display('price = $' + sale.price);
  boscode.display('tax @ ' + sale.taxRate + '% = $' + sale.tax);
  boscode.display('total cost = $' + sale.total);
};

sale = sale1;
calculateTax();
displaySale();

sale = sale2;
calculateTax();
displaySale();

sale = sale3;
calculateTax();
displaySale();
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/27/app.js`.
2. Add a fourth sale object.  
3. Update the code so that tax is calculated and the new sale is displayed.  
    Having two separate functions to calculate tax and display sales is good, each has a specific purpose. Having to call both functions for each sale object is not so good.
4. Can you change the code so that you don't have to call both functions for every sale?  
5. Paste your completed code into your google docs solution document.  



### 28 Updating our display function to add a blank line

##### Making code easier to read and update

As your programs get longer and more complicated, you manage that complexity by breaking them into well-named objects and functions. Anyone reading your code can follow its flow and understand the purpose of the pieces and of the whole.  

Take a look at the following code snippet; you should get a sense of what’s happening even if you don’t know the details of how the functions work.  

```js
...
var balance = getAccountBalance();
displayBalance();
addInterest()
addBonus();
setAccountBalance();
displayBalance();
...

```

Each function should have a single, clear purpose. If you need to investigate what a function does, you should be able to find it defined in one place. Let’s look at an example of updating a function.

```js
var boscode = require('boscode');

var movie1;
var movie2;
var movie3;
var movie;
var showMovieInfo;

movie1 = {
  title: 'Inside Out',
  actors: 'Amy Poehler, Bill Hader',
  directors: 'Pete Doctor, Ronaldo Del Carmen'
};

movie2 = {
  title: 'Spectre',
  actors: 'Daniel Craig, Christoph Waltz',
  directors: 'Sam Mendes'
};

movie3 = {
  title: 'Star Wars: Episode VII - The Force Awakens',
  actors: 'Harrison Ford, Mark Hamill, Carrie Fisher',
  directors: 'J.J.Abrams'
};

showMovieInfo = function () {
  boscode.display('Movie information for ' + movie.title);
  boscode.display('------------------------------');
  boscode.display('Actors: ' + movie.actors);
  boscode.display('Directors: ' + movie.directors);
  boscode.display('------------------------------');
  boscode.display('');
};

movie = movie1;
showMovieInfo();

movie = movie2;
showMovieInfo();

movie = movie3;
showMovieInfo();

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/28/app.js`.
2. Run the program.
3. Create three objects to represent blog posts.  
4. Create a function to display the posts on the console.  
5. Can you find your own way of visually separating the different blog posts on the console?
6. Paste your completed code into your google docs solution document.


### 29 A function to display player information


* A function is a block of code that you write once but use many times. It should have a clear, single purpose.

* You *define* a function by using the function keyword, parentheses and a function body in a code block between curly braces.

```js
function () {
    // statements go here in the function body
};
```

* You *assign* the function to a variable with the equals symbol, = , also known as the assignment operator.

```js
showPlayerInfo = function () { … };
```

* Once a function is assigned to a variable, you *call* or *invoke* the function by adding parentheses to the end of the variable name.

```js
addTax();
showPlayerInfo();
evadeRaptor();
```

* Be on the look out for repetition; sections of code with the same structure and only slight changes in values or variables used. Move repeated code into a function.

* Give functions clear names that communicate their purpose. Use the functions to organize your code, making your programs easier to follow and maintain.



```js
var boscode = require('boscode');

var player1;
var player2;
var player;
var showPlayerInfo;

player1 = {
  name: 'Kandra',
  place: 'The Dungeon of Doom',
  health: 50
};

player2 = {
  name: 'Dax',
  place: 'The Old Library',
  health: 40
};

showPlayerInfo = function () {
  boscode.display(player.name);
  boscode.display('------------------------------');
  boscode.display(player.name + ' is in ' + player.place);
  boscode.display(player.name + ' has health ' + player.health);
  boscode.display('------------------------------');
  boscode.display('');
};

player = player1;
showPlayerInfo();

player = player2;
showPlayerInfo();

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/29/app.js`.  
2. Run the program.  
3. Write a function that just shows where the player is.  
4. Write a function that just shows the player's health.  
5. Change the showPlayerInfo function to use your two functions.  
6. Paste your completed code into your google docs solution document.  



### 30 Relying on a variable outside of the function

Functions are an essential means of organization; you write them once and use them many times. But, so far, your functions have been tied to the values of variables around them. It is time to set your functions free, letting them name their own variables and passing them the data they need.  

The functions you have used so far have relied on variables declared and assigned values elsewhere in the program. In listing below, the showMessage function relies on a variable called message, declared outside of the function definition.

```js
var boscode = require('boscode');


var message;
var showMessage;

message = 'It\'s full of stars!';

showMessage = function () {
  boscode.display(message);
};

showMessage();
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/30/app.js`.  
2. Run the program.  
3. Change the message and run the program.  
4. Change the variable name in the parentheses for boscode.display. e.g. boscode.display(msg);
5. Run the program
6. Paste your completed code into your google docs solution document.


### 31 Passing information to a function

The instructions in the function body can use variables defined elsewhere in your program but that couples the function with the external variable; it’s generally better practice to pass the information a function needs to it when it is called. This helps avoid the variables a function needs being misnamed, missing, deleted or changed by other parts of your program and makes it easier to follow the flow of the program and spot mistakes if they occur.

We don’t want arrogant Rock God functions demanding particular variables in their dressing rooms before they’ll perform, we want easy going functions that are reliable and happy to strut their stuff wherever they are in the world. By de-coupling functions from variables, you make the functions more portable; the function definitions can be moved to other parts of your program, or be re-used in other programs or code libraries, without causing havoc and throwing errors.

So, how is this de-coupling achieved?

*Passing information to functions

Passing information to functions is achieved in two stages; when you define the function and whenever you call the function:  
1. When you *define* the function: you set up variable names, called *parameters*, ready for when you call the function.  
2. Whenever you *call* the function: you include data to assign to the variables you named in step 1.

*Passing one argument to a function

It’s time to make use of those empty parentheses in your function definitions! To pass information to functions when you call them, include it between the parentheses, like this:

```js
showMessage("It’s full of stars!");
showPlayerInfo("Kandra");
getMovieActors("The Hobbit");
square(12);
```

You pass each of the four functions some information for their code to use. Each value included in the parentheses is called an argument. Each of the four functions above includes a single argument. The arguments are “It’s full of stars!”, “Kandra”, “The Hobbit” and 12.  

To use the information in the parentheses, you need to make the functions ready to accept it. You add a parameter when you define the function. The parameter shows that the function expects you to give it some information when you call it.

For the four functions in the example above, the function definitions could be something like this:

```js
showMessage = function (message) { … };

showPlayerInfo = function (playerName) { … };

getMovieActors = function (movieTitle) { … };

square = function (numberToSquare) { … };
```


Each function definition includes a parameter, shown in bold. The parameter is a variable that you can only use inside the function body.

Let’s update the showMessage function from task 30 to accept a message, rather than relying on an external variable. When defining the function, include a message parameter. The message parameter is available as a variable in the function body. Now, when you call the function, you pass the message to display in parentheses, showMessage("It’s full of stars!"). The function adds some extra text and displays:

```js
var boscode = require('boscode');


var showMessage;

showMessage = function (message) {
  boscode.display('The message is: ' + message);
};

showMessage('It\'s full of stars!');

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/31/app.js`.  
2. Run the program.  
3. Change the message in the brackets when showMessage is called on line 11. The value in the brackets when showMessage is called is an argument. "It's full of stars!" was the original argument on line 11.  
4. Add two more calls to the showMessage function with different arguments each time.  
5. Paste your completed code into your google docs solution document.  


### 32 Calling the same function with different arguments

In listing below you call the showMessage function with three different arguments, leading to three different messages on the console.

```bash
> The message is: It’s full of stars!
> The message is: Hello to Jason Isaacs
> The message is: Hello to Jason Isaacs and Stephen Fry
```

js

```js
var boscode = require('boscode');

var showMessage;

showMessage = function (message) {
  boscode.display('The message is: ' + message);
};

showMessage('It\'s full of stars!');
showMessage('Hello to Jason Isaacs');
showMessage('Hello to Jason Isaacs and Stephen Fry');
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/32/app.js`.  
2. Run the program.  
3. Change the showMessage function to display its prefixed text on a separate line to the message.  
4. Declare a myMessage variable and assign it a string value.  
5. Call the showMessage function with myMessage as the argument.  
6. Paste your completed code into your google docs solution document.  


### 33 Using the square function

Because you declared the name of the parameter along with the function definition, the showMessage function no longer relies on variable names from elsewhere, making it less brittle. De-coupling complete.  

Listing below shows the definition of a square function, including a numberToSquare parameter. The function squares the number you pass to it as an argument. You call the function four times to give the following output:

```bash
> 10 * 10 = 100
> -2 * -2 = 4
> 1111 * 1111 = 1234321
> 0.5 * 0.5 = 0.25
```

js

```js
var boscode = require('boscode');

var square;

square = function (numberToSquare) {
  var result;
  result = numberToSquare * numberToSquare;
  boscode.display(numberToSquare + ' * ' + numberToSquare + ' = ' + result);
};

square(10);
square(-2);
square(1111);
square(0.5);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/33/app.js`.  
2. Run the program.  
3. Define a cube function that cubes any number passed in as an argument.
4. Call your cube function four times with different arguments to test it. 
5. Math.sqrt is a built-in function to find the positive square root of a number. e.g. Math.sqrt(9) finds the square root of 9. Define and test a squareRoot function to find square roots and display them on the console. e.g. The square root of 9 is 3.  
6. Paste your completed code into your google docs solution document.




### 34 A function with two arguments


* Parameters vs Arguments

You knew those parentheses would come in handy!  

The names you include in the parentheses *when defining the function* are available as variables in the function body. They are called *parameters* and show that you expect information to be included when the function is called.

```js
var myExample;

myExample = function (parameter) { … }
```

The values you include in the parentheses *when calling the function* are assigned to the parameter variables to be used in the function body. These values are called *arguments*.

```js
myExample(argument);
```

Don’t worry too much about the terminology; it can take a little while to get used to. After you’ve created and used a few functions, you’ll pick up an intuitive sense of what’s going on even if you mix up the terms parameter and argument from time to time.

*Passing multiple arguments to a function

You can define functions with as many parameters as they need to complete their work. Simply separate the parameters with commas in the parentheses of the definition.

```js
function (param1, param2, ...){
    //param1, param2, etc are available as variables in the function body
}
```


Suppose you want a function to add two numbers together. If you have two pairs of numbers, 30 and 23, and 2.8 and -5, the correct output would be

```bash
> The sum is 53
> The sum is -2.2
```

How do you do this?

Listing below: A function with two arguments

```js
var boscode = require('boscode');

var showSum;

showSum = function (number1, number2) {
  var total = number1 + number2;
  boscode.display('The sum is ' + total);
};

showSum(30, 23);
showSum(2.8, -5);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/34/app.js`.  
2. Run the program.  
3. Use the showSum function to add 56 and 74.  
4. To multiply two numbers, use the * symbol. e.g. 3 * 5 is 3 multiplied by 5. Create a showProduct function to multiply two numbers.
5. Use your function to multiply three pairs of numbers.
6. To divide one number by another, use /. e.g. 10 / 2 is 10 divided by 2. What about showDifference and showQuotient for subtraction and division?  
7. Paste your completed code into your google docs solution document.  


### 35 Displaying a player's name


You wrote a showPlayerInfo function as ‘code on demand.’ You could display player information on the console whenever you wanted, just by calling the function. Unfortunately, it relied on a player variable being set elsewhere in the code. Let’s update the showPlayerInfo function, setting parameters so you can pass it the information it needs directly.  

In order to display information about each player, you break the job into sub-tasks and create functions for each piece of information. You then show information about a player like this:  

```bash
showPlayerName("Kandra");
showPlayerHealth("Kandra", 50);
showPlayerPlace("Kandra", "The Dungeon of Doom");
```

Each function has a very specific job to do. If you want to display all of the information at once, you wrap the individual functions inside one master function and pass it all the information it needs:

```bash
showPlayerInfo("Kandra", "The Dungeon of Doom", 50);
```


Your first function’s job is to simply display the player’s name. That’s it. No bells or whistles. Listing below shows the showPlayerName function definition and calls the function with two different names to produce the following output:

```bash
> Kandra
> Dax
```

js

```js
var boscode = require('boscode');

var showPlayerName;

showPlayerName = function (playerName) {
  boscode.display(playerName);
};

showPlayerName('Kandra');
showPlayerName('Dax');
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/35/app.js`.  
2. Run the program.  
3. Update the text logged so that it is of the form: The player's name is Kandra.  
4. Strings have a length property that gives the number of characters in the string. e.g. `playerName.length`. Make the function show the number of letters in the player's name.  
5. Paste your completed code into your google docs solution document.



### 36 Displaying a player's name via an object property


You’re not likely to call the showPlayerName function with literal values like "Kandra" and "Dax". You’re much more likely to use variables. In particular, JavaScript objects will represent players. Listing below updates the code to use a couple of player objects instead. 


```js
var boscode = require('boscode');

var player1;
var player2;
var showPlayerName;

showPlayerName = function (playerName) {
  boscode.display(playerName);
};

player1 = {
  name: 'Kandra',
  place: 'The Dungeon of Doom',
  health: 50
};

player2 = {
  name: 'Dax',
  place: 'The Old Library',
  health: 40
};

showPlayerName(player1.name);
showPlayerName(player2.name);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/36/app.js`.
2. Run the program.
3. In the showPlayerName function, change playerName to playerName.toUpperCase(). Run the function.
4. Change the function to show the player's name in lower case.
5. Paste your completed code into your google docs solution document.



### 37 Displaying a player's health

The showPlayerHealth function definition includes two parameters, playerName and playerHealth, to produce output like this:

```bash
> Kandra has health 50
> Dax has health 40
```

js

```js
var boscode = require('boscode');

var showPlayerHealth;

showPlayerHealth = function (playerName, playerHealth) {
  boscode.display(playerName + ' has health ' + playerHealth);
};

showPlayerHealth('Kandra', 50);
showPlayerHealth('Dax', 40);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/37/app.js`.  
2. Run the program.  
3. Change the showPlayerHealth function so it shows information of the form: Kandra: health 50.  
4. Call the showPlayerHealth function using your own arguments.  
5. Declare a variable called healthInfo inside the showPlayerHealth function.  
  `var healthInfo;`  
6. Assign healthInfo the string that will be displayed.   
  `healthInfo = playerName + ': health ' + playerHealth;`  
7. Change the call to boscode.display so that it uses the `healthInfo` variable.  
8. Paste your completed code into your google docs solution document.  



### 38 Displaying a player's health via object properties

The call to showPlayerHealth in listing above used the literal values "Kandra" and 50. In the final program, each player’s information is assigned to the properties of a player object. Your calls to showPlayerHealth are much more likely to use those properties rather than hard-coded values. Listing below updates the code to include player objects.


```js
var boscode = require('boscode');

var player1;
var player2;
var showPlayerHealth;

showPlayerHealth = function (playerName, playerHealth) {
  boscode.display(playerName + ' has health ' + playerHealth);
};

player1 = {
  name: 'Kandra',
  place: 'The Dungeon of Doom',
  health: 50
};

player2 = {
  name: 'Dax',
  place: 'The Old Library',
  health: 40
};

showPlayerHealth(player1.name, player1.health);
showPlayerHealth(player2.name, player2.health);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/38/app.js`.  
2. Run the program.  
3. Add a new property to the player objects called healthMultiplier.  
4. Add a third parameter to the definition of the showPlayerHealth function called playerHealthMultiplier.  
5. Update the function so that the health displayed is first multiplied by the health multiplier.  
6. Add the player's healthMultiplier property as a third argument to the two calls to the showPlayerHealth function.  
7. Paste your completed code into your google docs solution document.  



### 39 Displaying a player's location

Name: check. Health: check. That just leaves location.


The showPlayerPlace function definition also includes two parameters, this time playerName and playerPlace, and produces output like this:

```bash
> Kandra is in The Dungeon of Doom
> Dax is in The Old Library
```

js

```js
var boscode = require('boscode');

var showPlayerPlace;

showPlayerPlace = function (playerName, playerPlace) {
  boscode.display(playerName + ' is in ' + playerPlace);
};

showPlayerPlace('Kandra', 'The Dungeon of Doom');
showPlayerPlace('Dax', 'The Old Library');
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/39/app.js`.
2. Run the program.
3. Inside the boscode.display parentheses, change playerName to playerName[0]. Run the program. What effect do the brackets have?
4. Change the number in the brackets to 1.
5. What happens when you change the number to 3? Why?
6. Paste your completed code into your google docs solution document.



### 40 Displaying a player's location via object properties

And once again, switching from the hard-coded literal values in listing above to object properties gives you an updated version in listing below.


```js
var boscode = require('boscode');

var player1;
var player2;
var showPlayerPlace;

showPlayerPlace = function (playerName, playerPlace) {
  boscode.display(playerName + ' is in ' + playerPlace);
};

player1 = {
  name: 'Kandra',
  place: 'The Dungeon of Doom',
  health: 50
};

player2 = {
  name: 'Dax',
  place: 'The Old Library',
  health: 40
};

showPlayerPlace(player1.name, player1.place);
showPlayerPlace(player2.name, player2.place);
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/40/app.js`.  
2. Run the program.  
3. In the boscode.display parentheses, change `playerName` to `playerName.substring(0, 1)`. Run the program. What do you think the substring function does?  
4. Change the arguments to the substring function to (0, 2), then (0, 3) and so on.  
5. Change the arguments to (1, 2), then (1, 3) and so on.  
6. What role do you think the two arguments to the substring function have?  
7. Paste your completed code into your google docs solution document.  





### 41 Displaying a player's information


The showPlayerInfo function uses your three individual functions, showPlayerName, showPlayerHealth and showPlayerPlace, and adds a touch of formatting to produce a display of each player’s properties. The output for one player looks like this:

```bash
>
> Kandra
> ----------------------------
> Kandra is in The Dungeon of Doom
> Kandra has health 50
> ----------------------------
```


js

```js
var boscode = require('boscode');

var showPlayerInfo;
var showPlayerName;
var showPlayerHealth;
var showPlayerPlace;

showPlayerName = function (playerName) {
  boscode.display(playerName);
};

showPlayerHealth = function (playerName, playerHealth) {
  boscode.display(playerName + ' has health ' + playerHealth);
};

showPlayerPlace = function (playerName, playerPlace) {
  boscode.display(playerName + ' is in ' + playerPlace);
};

showPlayerInfo = function (playerName, playerPlace, playerHealth) {
  boscode.display('');

  showPlayerName(playerName);

  boscode.display('----------------------------');

  showPlayerPlace(playerName, playerPlace);
  showPlayerHealth(playerName, playerHealth);

  boscode.display('----------------------------');
  boscode.display('');
};

showPlayerInfo('Kandra', 'The Dungeon of Doom', 50);
showPlayerInfo('Dax', 'The Old Library', 40);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/41/app.js`.  
2. Run the program.  
3. Create a function called showLine that displays a line of dashes to the console. `----------------------------`  
4. Update the showPlayerInfo function to use the showLine function rather than logging dashes to the console directly.  
5. Create and use a showBlankLine function for logging a blank line to the console.  
6. Paste your completed code into your google docs solution document.  



### 42 Displaying a player's information using properties


You call the showPlayerInfo function with three arguments each time. It, in turn, passes the required arguments on to the showPlayerName, showPlayerHealth and showPlayerPlace functions.  

You end with all the pieces put together in a single listing. It includes each variable declaration and assignment as a single step and uses player object properties, like player1.name, rather than literal values, like "Kandra", when calling showPlayerInfo.  


```js
var boscode = require('boscode');

var showPlayerName = function (playerName) {
  boscode.display(playerName);
};

var showPlayerHealth = function (playerName, playerHealth) {
  boscode.display(playerName + ' has health ' + playerHealth);
};

var showPlayerPlace = function (playerName, playerPlace) {
  boscode.display(playerName + ' is in ' + playerPlace);
};

var showPlayerInfo = function (playerName, playerPlace, playerHealth) {
  boscode.display('');

  showPlayerName(playerName);

  boscode.display('----------------------------');

  showPlayerPlace(playerName, playerPlace);
  showPlayerHealth(playerName, playerHealth);

  boscode.display('----------------------------');
  boscode.display('');
};

var player1 = {
  name: 'Kandra',
  place: 'The Dungeon of Doom',
  health: 50
};

var player2 = {
  name: 'Dax',
  place: 'The Old Library',
  health: 40
};

showPlayerInfo(player1.name, player1.place, player1.health);
showPlayerInfo(player2.name, player2.place, player2.health);

```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/42/app.js`.
2. Run the program.
3. Define a showLine function with a parameter for the length of line. e.g. `showLine(5)` should output  
  `----- `  
  `showLine(20)` should output  
  `--------------------`  
  *    Hints:  
  a) In the function body declare a line variable and assign it a long string of dashes.  
  b) Use the substring function to grab a line of the correct length. line.substring(0, 10) would have length 10.  
4. Use your showLine function to display the player's name in a box.  
  `----------`  
  `- Kandra -`  
  `__________`  
5. Update your showLine function to use asterisks rather than dashes.  
  `**********`  
  `* Kandra *`  
  `**********`  
6. Paste your completed code into your google docs solution document.  






### 43


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/43/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 44


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/44/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 45


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/45/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 46


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/46/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 47


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/47/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 48


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/48/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 49


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/49/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.





### 50


```js
```

###### The challenge:

1. In your cloud 9 workspace edit the file  `/home/ubuntu/workspace/code/computingclub/50/app.js`.
2. Run the program.

. Paste your completed code into your google docs solution document.







