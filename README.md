# Term 3 Week 1 Notes
##### How to format a readme - https://help.github.com/articles/basic-writing-and-formatting-syntax/

## What the fuck is Javascript? - https://organicdonut.com/2013/08/technical-understanding-javascript-node-js-and-their-libraries/

### Javascript
> JS is a programming language for use in web browsers, it was once a "scripting language", now it is just a full language.
> It is used to maniuplate the DOM or "Document Object Model". The elements on a webpage.
> It is fully client side. The browser handles and runs the code, everything happens inside a sandbox.

### AJAX
> AJAX stands for "Asynchronous Javascript and XML".
> It is a for webpages to send and recieve data without refreshing the page.
> XML is a markup language like HTML.
> Has uses in combination with JSON and it allows us to package the data properly, then utlise AJAX with it.

### jQuery
> jQuery is a library built for JS to automate and simplify common tasks.
> Took off as it was so useful with old browsers.
> Mainly used for animation and AJAX, which are difficult to do with vanilla JS.

### AngularJS
> Angular is a full frontend MVC framework for JS web apps.
> Built by google.
> Provides a quick way of building large single page web apps.
> Included on pages like jQuery inside <script> tags.
> Unlike jQuery though, it is meant to be used as a full framework for an entire web app to use.
> In order to understand Angular, you need to get JS first, as it requires a deep understanding of prototyping, scope and other vanilla JS aspects.

### Node.js
> Does not run in thw browser.
> Command line tool that runs JS on a machine without needing to run in the browser.
> Before Node.js, developers had to use different lanugages for the back end, like PHP, Java or ASP.net.
> Now Node.js allows people to learn one language only.

### Summary
>JavaScript is a language written for websites to run in the client’s browser.

>AJAX is a way for JavaScript to request data from a server without refreshing the page or blocking the application.

>jQuery is a JavaScript library built to automate and simplify common web tasks like AJAX or animation.

>Angular is a hip JavaScript framework which is made for building large, single-page web applications.

>Node.js allows JavaScript to be run without a browser, and is commonly used to run web servers.

## Day 1 - Monday 5th Nov

>Going through some node stuff today, first day of learning MEAN stack. Have installed new docsets for various JS languages.

###https://nodejs.org/en/
> Node.js home page

###https://github.com/creationix/nvm
> Install NVM according to instructions, from here, install node via NVM install node

###https://trello.com/b/BVujtxWF/term-3-javascript-node-mongodb-react
> Trello board of JS challenges for completion in the afternoon.

###https://www.developphp.com/video/JavaScript/Digital-Clock-Tutorial-Custom-Animated-Clock
> Tutorial used to complete the digital clock challenge
> GH Link: https://github.com/JohnVonNeumann/digital-clock_js.git

###https://github.com/getify/You-Dont-Know-JS
> Free online book with challenges similar to that of LRTHW or Michael Hartl's Rails stuff, working through some of the challenges.


## Day 2 - Tuesday 6th Nov

>Today our lecture is on Callback Functions.

### Reading through EJS - http://eloquentjavascript.net/01_values.html

> Bits are organised and represented as 0's or 1's. In this case, creating numbers in binary operates by using powers of 2, each digit from right to left increases the "underlying value we seek in legitimate humanly understood numbers" by a factor of two.

#### An example of the number 431 in binary:

> 512 | 256 | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
>  0  |  1  |  1  | 0  | 1  | 0  | 1 | 1 | 1 | 1 |
__________________________________________________
> 431 = 0110101111

> Using, JavaScript can display number values upto 18 quintillion, which is an 18 with 18 zeroes after it, JS performs this numerical representation by restricting its binary digit string length to 64 bits.
#### Basic value types in js:
* numbers
* strings
* booleans
* objects
* functions   
* undefined values


## Day 3 - Wednesday 7th Nov

> Setting up Node.js files, using 'npm init' and fill out the relevant info using enter and inputting info, at the end, it will output a json fle called package.json.

> We then run 'npm install node-fetch --save' to add a fetch package to our dir, this adds a folder called 'node_modules' to our file tree in atom, thhe 'npm WARN xxxxxxxxx No repository field' comment is apparently normal.

### JQuery
>Old, around a decade old.
>jQuery wraps common DOM and JS tasks to be more friendly.
>jQuery is JS.
>It is not a framework, it is a library.
>jQuery is NOT vanilla JS.
>jQuery is being phased out due to younger frameworks doing it's job in less code.

### API - Application Programming Interface
>Allows us to write code that generates an interface to interact with.

### Node.js Youtube Explanation - https://www.youtube.com/watch?v=KsjrN-T3ZCs&index=3&list=PL6gx4Cwl9DGBMdkKFn3HasZnnAqVjzHn_#t=135.81712

### Node.js Video Notes

#### when we use == vs ===
* == compares values
> for example: 'console.log(19 == "19"); // true '
* === compares values AND types
> for example: 'console.log(19 === "19"); // false '

#### this - https://youtu.be/uiZxziF4Ol8?list=PL6gx4Cwl9DGBMdkKFn3HasZnnAqVjzHn_

> when we call 'this', it only refers to the thing that called it
> 'this' is the js equivalent of 'self' in ruby, it's similar to that of an instance var, basically
> it's default is a global call, as if it is not being called by something, it reverts to global calling.
> an example, Louis.printFirstName(); // 'this' is called on Louis.
> an example, printFirstName();       // 'this' is called globally

#### prototype - https://youtu.be/IW2M8G8uJ6o?list=PL6gx4Cwl9DGBMdkKFn3HasZnnAqVjzHn_

>prototyping allows us to add functions on the fly to models we've already created
> example: User.prototype.magic  = 60;
> User would have been previously created, it allows us to create a new function that pertains to a model without having to edit the original model
