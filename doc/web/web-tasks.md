# Web tasks

## Table of Content

[Installation](#installation)     

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

3. Open `https://web-{yourname}.c9users.io/01_Hello_world/` in Google Chrome  and and also open the developer tools: Windows: F12 or Ctrl-shift+I, Mac: Cmd + Opt + I.
4. Click the button and observe the console output.

###### The challenge:

Modify program.js to multiply 34 with 42


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

3. Open `https://web-{yourname}.c9users.io/01_Hello_world/` in Google Chrome  and and also open the developer tools: Windows: F12 or Ctrl-shift+I, Mac: Cmd + Opt + I.
4. Click the button and observe the console output.

###### The challenge:
