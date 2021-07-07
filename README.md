<!DOCTYPE html>
<html>
    <!--
    *********Welcome*********
    Welcome, if you are here to learn about something referenced in one of my coding challenges or in Primavera then feel free to use this documentation for any purposes you have in mind!
    
    Happy coding! :-)
    
    Note: Some of the tutorials here are year(s) old & may not be completely up-to-date or accurate.
    -->
    <head>
        <meta charset="utf-8">
        <title>IP's Documentation.</title>
        <link href="https://fonts.googleapis.com/css?family=Material+Icons|Merriweather|Fjalla+One|Abril+Fatface&display=swap" rel="stylesheet">
        <style>
            /* Changing the body in a few ways */
            body {
                background-color: rgb(255, 255, 255);
                margin: 0px;
                color: black;
                font-family: "Abril Fatface", sans-serif;
            }
            
            /* Styling each of the page containers */
            #program-name, .page-container {
                text-align: center;
            }
            .page-container {
                background-color: rgba(0, 0, 225, 0.5);
                border: 10px double rgb(0, 0, 200);
                border-radius: 5px;
                -webkit-border-radius: 5px;
                -moz-border-radius: 5px;
                margin-left: 75px;
                width: 405px;
                padding: 10px;
            }
            .page-container p {
                font-family: 'Fjalla One', sans-serif;
            }
            
            /* Styling the button class */
            .buttons {
                background-color: blue;
                color: black;
                border: none;
                border-radius: 0px;
                transition: border-radius 1s ease;
            }
            .buttons:hover {
                cursor: pointer;
                border-radius: 25px;
                transition: border-radius 1s ease;
            }
            
            /* Styling the button group*/
            .btn-group {
                margin-left: 190px;
                margin-bottom: 10px;
            }
            .btn-group .button i {
                margin-top: 8px;
                margin-left: 0%;
                transition: margin-left 1s ease;
            }
            .btn-group .button:hover i {
                margin-left: 50%;
                transition: margin-left 1s ease;
            }
            .btn-group .button span {
                margin-left: 10px;
                margin-top: 10px;
                position: absolute;
            }
            .btn-group .button {
                background-color: rgb(0, 60, 200); 
                font-size: 16px;
                border: 1px solid rgb(0, 0, 100); 
                height: 40px;
                color: white; 
                padding: 0px 0px 8px 0px;
                cursor: pointer; 
                float: left; 
                width: 70px;
                transition: width 0.5s ease;
            }
            .btn-group .button:not(:last-child) {
                border-right: none; 
            }
            /* Clear floats (clearfix hack) */
            .btn-group:after {
                content: "";
                clear: both;
                display: table;
            }
            .btn-group .button:hover {
                background-color: rgb(0, 60, 225);
                width: 90px;
                transition: width 0.5s ease;
            }

            /* Drop down buttons */
            .dropbtn {
                background-color: #3498DB;
                color: white;
                padding: 16px;
                border: none;
                cursor: pointer;
            }
            .dropdown {
                float: left;
                position: relative;
                display: inline-block;
            }
            .dropdown-content {
                display: none;
                position: absolute;
                top: 40px;
                right: -5px;
                z-index: 1;
            }
            .show {
                display: block;
            }
            /**Removing the default focus from buttons**/
            .button:focus, .buttons:focus {
                outline: none;
            }
            
            /* Preventing icons and special texts from getting in the way of hovering over the button which they're in */
            i, span {
                pointer-events: none;
            }
            
            /* Styles the notes page */
            #search-bar {
                padding: 6px;
                border: 2px solid grey;
                margin-top: 0px;
                margin-right: 37.5px;
                width: 223.5px;
                font-size: 17px;
            }
            #search-bar:focus {
                outline: none;
            }
            #search-icon {
                background-color: white;
                border: 2px solid grey;
                width: 32px;
                padding-top: 4px;
                height: 28px;
                position: absolute;
                left: 395px;
                top: 247px;
            }
            #search-icon:hover {
                cursor: pointer;
            }
            #search-note {
                margin-top: 0px;
                margin-bottom: 5px;
                font-size: 11.5px;
                font-family: "Merriweather", sans-serif;
            }
            #look-note {
                margin-top: 25px;
                margin-bottom: 5px;
                font-size: 11.5px;
                font-family: "Merriweather", sans-serif;
            }
            .search-results {
                background-color: rgba(255, 255, 255);
                margin-left: 66px;
                width: 268px;
                height: 25px;
                color: black;
            }
            .search-results:hover {
                background-color: rgba(200, 200, 200);
                cursor: pointer;
            }
            .back-button {
                background-color: blue;
                position: absolute;
                left: 100px;
                top: 200px;
            }
            /* Notes */
            .code {
                background-color: rgb(200, 200, 200);
                margin: 20px;
                border: 1px solid rgba(0, 0, 0, 0.3);
                text-align: left;
                padding: 10px;
                white-space: pre-wrap;
            }
            
            .comment {
                color: rgb(35, 150, 70);
            }
            
            .important-comment {
                color: rgb(44, 44, 232);
            }
            
            .new-code {
                color: rgb(200, 0, 0);
            }
            
            /* Styles the news page */
            .new-post {
                background-color: rgba(255, 255, 255, 0.3);
                border: 5px solid black;
                width: 300px;
                margin-left: 40px;
                margin-top: 25px;
                padding: 5px;
            }
            .post-date {
                border: 2px dashed black;
                margin-bottom: 5px;
            }
            .post-info, .post-date, #news-welcome {
                font-family: "Merriweather", sans-serif;
            }
            
            /* Styling the owner text */
            #owner-text {
                margin-left: 160px;
                margin-bottom: 5px;
            }
            
            .table-of-contents {
                text-align: left;
            }
            
        </style>
    </head>
    <body>
    <!--Material Icons here: https://material.io/resources/icons/?icon=image&style=baseline-->
        <!--Part of the webpage that is always visible-->
        <div id="header">
            <h1 id="program-name">Iron's Documentation</h1>
        
            <!--A group of buttons-->
            <div class="btn-group" style="width:60%">
                <!--Home button-->
                <button id="home-button" class="button"><span class="home-hide">Home</span><i class="material-icons">house</i></button>
                <!--Groups button-->
                <button id="note-button" class="button"><span class="note-hide">Notes</span><i class="material-icons">
assignment</i></button>
                <!--News button-->
                <button id="news-button" class="button"><span class="news-hide">News</span><i class="material-icons">new_releases</i></button>
            </div>
        </div>
        
        <!--Home-->
        <div id="home-page">
            <div class="page-container">
                <h2 class="page-name">Home</h2>
                <p>Welcome to Iron Programming's Documentation. This is where I store basic tutorials of coding mechanics & techniques. If you are here from one of my coding challenges or from Primavera then take a look around to find what you are looking fore.</p>
                <h4>How to use</h4>
                <p>Simply go to the articles, and scroll through them to find the one that you are looking for. You can also use the search bar if you wish.</p>
            </div>
        </div>
        
        <!--Note book-->
        <div id="note-page">
            <div class="page-container">
                <h2 class="page-name">Programming Notebook</h2>
                
                <!--Looking for the notes-->
                <div id="tutorials">
                    <!--Search bar-->
                    <div id="search-place">
                        <!--<h5 id="search-note">Search through my notes to find an example of what you're looking for.</h5>
                        <input id="search-bar" type="text" placeholder="Search...">-->
                    </div>
                    
                    <!--<div id="search-icon">
                        <i class="material-icons">search</i>
                    </div>-->
                    
                    <!--Choosing from the available options-->
                    <h5 id="look-note">Didn't find what you were looking for? Ask me any questions you have, and I'll do my best to answer you!</h5>
                    
                </div>
                
                <!--Reading the notes that you clicked on-->
                <div id="read-notes">
                    <button class="buttons back-button"><i class="material-icons">arrow_back</i></button>
                </div>
                
                <!--Search results when you press enter or click on the magnifying glass-->
                <div id="searchResults">
                    <h5>Search results</h5>
                    <button class="buttons back-button"><i class="material-icons">arrow_back</i></button>
                    <p id="searchFalse">No results matching your search have been found.</p>
                </div>
                
            </div>
        </div>
        
        <!--News-->
        <div id="news-page">
            <div class="page-container">
                <h2 class="page-name">News and Updates</h2>
                <h6 id="news-welcome">Updates on Iron's Documentation.</h6>
                <ul class="table-of-contents">
                    <li><a href="#first-post">Introduction</a></li>
                </ul>
                <!--First Post-->
                <div class="new-post" id="first-post">
                    <h4>Introduction</h4>
                    <p class="post-info">Hey everyone, I'll post things here if I feel the need to.</p> 
                    <p class="post-date">Sunday, October 4, 2020</p>
                </div>
            </div>
        </div>
        
        <!--Storage text for the tutorials-->
        <div id="storage-notes">
            <!--Processing Java Script Tutorials-->
            <pre class="code" id="lerpColor">
/*****Processing Java Script: LerpColor*****/
/** 
 * lerpColor(c1, c2, amount); 
 * Combines to colors. amount is any number from 0 to 1 representing 0 to 100%. 
 * It is the equivalent of mixing two colors together in RGB color science. 
**/ 

var R = color(255, 0, 0), G = color(0, 255, 0); 
var Mix = lerpColor(R, G, 0.5); // what happens when we mix red and green evenly?

// resulting color 
fill(Mix); 
rect(175, 25, 50, 50); 

// The word "gradient" means a gradually change. So a color gradient is a transition of colors. 
strokeWeight(1); 
for (var i = 0; i &lt; 300; i++) { 
    // since we are iterating from i=0 to i=300 we want our percentage of colors to slowly transition from our "R" color to our "G" color. We can do this by dividing i by the the last iteration (300). When i=0 we get 0/300 = 0, completley red. When i=300 we get 300/300=1, completely green. 
    var COL = lerpColor(R, G, i / 300); 
    stroke(COL); 
    // note that I translate the line down so we can still see the greenish-red square 
    line(0, i + 100, 400, i + 100); 
}
            </pre><!--LerpColor-->
            <pre class="code" id="PJS-Shapes">
/*****Processing Java Script Shapes*****/

/*
*** Argument Conventions ***
* x = how far to the right of the screen,
* y how far to the bottom of the screen
* width/height = size of the shape
* radius how curved the corner of the shape is
*/

// Drawing a rectangle (* means optional parameter)
rect(x, y, width, height, *radius);

// Drawing an ellipse
ellipse(x, y, width, height);

// Drawing a triangle
triangle(x1, y1, x2, y2, x3, y3);

// If you want to draw a rectangle with different amounts of radius of different corners of the rectangle, you can do it like this;
(rect)(x, y, width, height, radius1, radius2, radius3, radius4);

// Drawing more complex shapes
If you're interested in making more crazy shapes, check out the following functions in KA's Documentation under your program; 
- bezier();
- beginShape();/endShape();
- curveVertex();/vertex();/bezierVertex();


            </pre><!--Shapes-->
            <pre class="code" id="Text">
/*****Processing Java Script Text*****/

/*
*** Argument Conventions ***
* message = the text of the message, can either be a string ("Message") or a number (1, 2, ect)
* x = how far to the right of the screen,
* y how far to the bottom of the screen
* width/height = the maximum capacity of the text block, if the text overflows the text will break into the next line (like pressing enter)
*/

// Drawing text (width and height are optional)
text(message, x, y, *width, *height);

/**
A few other tricks when using text are:
1. \n = Make an line break.
2. "Jack: \"Hello!\"." //The \" means that the quotation marks is not ending the message, instead, it's meant to be a part of the message.
**/
            </pre><!--Text-->
            <pre class="code" id="Variables">
/***********Variables***********/
/*
* Variables are things we define that can be reused later, as well as being able to be changed. 
* There are many ways we can define variables as, here are a few ways; 
    1. Strings -> "This is a string"
    2. Numbers (storing values) -> 12349 
    3. Boolean Values -> true/false
    4. Functions -> We can define functions
    5. Objects -> We can define objects
    6. Arrays -> We can define arrays
*/

// Defining a variable
var xPosition = 25;

// Using that variable
ellipse(xPosition, 25, 25, 25);


// We can define multiple variables at the same time separating variables by a comma;
var xPosition = 25, yPosition = 25, size = 50;

// Using those variables
ellipse(xPosition, yPosition, size, size);

/*
* Make sure not to define multiple variables using the same name!
* Variables can be changed due to events like in a draw() function.
* There are two types of variables; local and global. Local variables are defined within a function, loop, or some other Java Script element. These variables can only be accessed within that Java Script element. The other type is called a global variable which means its not defined within some Java Script Element which would limit its range.
*/

            </pre><!--Variables-->
            <pre class="code" id="Animation">
/**
*********Animation (Moving things)*********
1. To animate anything, you always need a draw function;
draw = function() {
   //In a draw function, everything is repeated over and over again. Thus enabling us to animate things.
};

2. Before we do anything else, we need to declare a variable that we can increase, let's say "SquareXPos":
var SquareXPos = 50;

draw = function() {
    
};

3. Now we can add a background, and then draw the black square
var SquareXPos = 50;

draw = function() {
    background(255, 255, 255);//White background
    //Black square
    fill(0, 0, 0);
    rect(SquareXPos, 200, 50, 50);
};

4. Now we need to increase the "SquareXPos" to move the car in the x direction, we do that by saying; "SquareXPos += amountPerMilisecond" in the draw function. So if we wanted to move the black square 5 in the x direciton every millisecond, then we would say; 
"SquareXPos += 5;". Now we have:
**/
var SquareXPos = 50;
draw = function() {
    background(255, 255, 255);//White background
    //Black square
    fill(0, 0, 0);
    rect(SquareXPos, 200, 50, 50);
    
    SquareXPos += 5;
};

/*
* If you had the "background();" outside of the draw function like this
background(255, 255, 255);
draw = function() {
    //Stuff
};
Then even though the black square would move, it look like someone was painting (because the background is not being drawn repeatedly over and over again to cover up the old square's postions).

* Don't define variables inside the draw() function, if you do the variables will be re-defined every single frame!

* Shortcut for animating; We can use "SquareXPos++;" instead of  "SquareXPos += 1;" if we are increasing by 1.**/
            </pre><!--Animation-->
            <pre class="code" id="Operations">
/**
*********Operations*********
* Here's how to use the following operations:
* The multiplication symbol *, simply multiplies the two numbers.
* The division symbol /, simply divides the first number by the second.
* The addition symbol +, simply adds the two numbers.
* The subtraction symbol -, simply subtracts the second number from the first.
* The percent symbol %, divides the first number by the second, but returns the remainder instead of the exact answer.
* The random(num1, num2) function gets a random number between num1 and num2. If you leave the parenthesis empty, it gets a random number between 0 and 1, if you put in one number, it gets a number between 0 and that number. 
* To round a number to the nearest integer, simply use the round(number) function.
* To round a number to the next highest integer, simply use the ceil(number) function.
* To round a number to the next lowest integer, simply use the floor(number) function.
* The map(x, x1, x3, y1, y2) function, finds the equation of a line (based off the the line coorinates you gave), and then returns a position on the line corresponding to the "x" value.
* &lt;&lt;&lt;, >>>, &lt;&lt;, >> are binary operators. They essentially change the binary form of the number by moving all the 0's and 1's one space forward or backward. For more info you can ask how they work in the Questions section.
**/
            </pre><!--Operations-->
            <pre class="code" id="IIFE">
/*
* Using IIFE (Immediately Invoked Function Expression) *
*/
var functionName = (function() {
    
})(); 
/** we include the first parenthesis; 
* there > (function() {}) &lt; and there as a precaution
* the final parenthesis () right before the semicolon is what automatically invokes the functions 
**/

// Using return, we can do some pretty powerful things with this;
1. Returning an image
var functionName = (function() {
    background(0, 0, 0, 0);
    fill(255, 0, 0);
    rect(0, 0, 25, 25);
    return get(0, 0, 25, 25); // returning an image so we can reference this function as an image
})();

image(functionName, x, y);

2. Returning a function (this is useful to help organize related code); as well as being a bit faster I believe
var functionName = (function() {
    // define some related variables

    var otherFunction = function() {
        // do stuff
    };
    
    return otherFunction
})();
            </pre><!--IIFE-->
            <pre class="code" id="Functions">
/**
*********Functions*********
* A function is a type of variable and gives us a way to store code that we can draw later.
* 
* In the "Processing Java Script" environment that KA has for us, we have simple functions like "ellipse" or "rect" pre-defined for us.
**/

1. 
// To create a function we do like so;
var FunctionName = function() {
    // code in here
    fill(0, 0, 0);
    rect(150, 150, 25, 25);
};

//And then to call the function (which writes it code)
FunctionName();

2. We can fill the function's parenthesis with parameters which are considered local variables;
var functionName = function(xPosition, yPosition, Size, Color) {
    // code in here
    fill(Color);
    rect(xPosition, yPosition, Size, Size);
};

// Then when we call the function, we fill in its arguments (the local variables/paramters in its parenthesis); 
functionName(25, 25, 50, color(0, 200, 0));

// color(r, g, b) is like fill(r, g, b) with the exception that color() can be used as an argument, while as fill() can't.

/*
* If we wish to stop the function's execution, we can use return;
*/

// example
var functionName = function() {
    // do stuff, 
    return; // this would stop the function's execution before the rest of the code is executed
    // do stuff
};

// We can also return "something". For an example;
var functionName = function() {
    return "Returned String";
};

// Which if we called that function it would be the same as calling a string; 
text(functionName(), 25, 25); // drawing "Returned String" at (25, 25)
            </pre><!--Functions-->
            <pre class="code" id="Conditions">
/***********Conditional Statement***********/

// To check if something is true or not, we can use an "if statement";
if (somethingIsTrue) {
    // do something
}

// Then, if we want to do another check if the first is not true, we can use an "else if" or "else" statement;
if (somethingIsTrue) {
    // do something
} else if (somethingElseIsTrue) {
    // do something else
} else { // else if none of the above is true
    // do something else
}

/*
* A boolean expression is an expression that evaluates to either true or false. That is the type of expression we put into a conditional statement. Here are some examples of what we can do;
1. Equality (===) for numbers; 
if (something === 1) {// Do something}
2. Equality (===) for strings;
if (something === "This String") {// Do something}
3. Equality (===) for boolean values
if (something === true) {// Do something}
4. Inequality (&lt; OR > OR &lt;= OR >=) for numbers;
if (something &lt; 25) {// Do something}
5. Shortcut for boolean values
"if (something) {}" instead of "if (something === true) {}"
"if (!something) {}" instead of "if (something === false) {}"
*/

/*Combined boolean statements (we use && to combine two boolean statements; if their both true, then evaluate the code inside the if statement)*/
if (something === 1 && somethingElse === true) {// Do something}

/*Combined boolean statements (we use || to combine two boolean statements; if either of them are true, then evaluate the code inside the if statement)*/
if (something === 1 || somethingElse === true) {// Do something}


/** Using switch, case, and break **/
//Another type of conditional statement is switch/case/break

// switch the otucome depending on the value of the variable
switch (variable) {
    // if variable equals 0, then evaluate the code inside
    case 0:
        // code
    break; // if the code inside that first option is run, take a break and stop executing the switch() {} statement
    case 1: // otherwise, keep checking
        // code
    break;
    case 2: 
        // code
    break;
    
    default: 
        // draw some default code if none of the above is true
}

// NOTE: for the last case or default statement you don't need a break statement, as shown above


/* Shortened if/else statement */
// define out variable (as nothing)
var variable;

// this 
variable = (condition) ? outcome1 : outcome2;

// is the same thing as this;
if (condition) {
    variable = outcome1;
} else {
    variable = outcome2;
}
            </pre><!--Conditions-->
            <pre class="code" id="Loops">
/**********Loops**********/
/**
* A loop repeats the code inside of it a certain number of times
* There are two types of loops, for and while
**/

1. USING THE FOR LOOP
// In a for loop, we combine 3 steps in one;
First, define the variable "var i = startValue", (semicolon)
Second, we put a limit on how big or small the variable can get, (semicolon)
Third, we increase that variable by a certain amount until it is bigger than the "number"
for (var i = startValue; i&lt; endValue; i += incrementValue) {
    // code to repeat
}

// EXAMPLE: Drawing a line of 5 rectangles in the horizontal direction
fill(255, 0, 0);
for (var i = 0; i &lt; 5; i++) {
    rect(25 + (i * 25), 25, 25, 25);
}

// NOTE: I used the variable "i" because it is nice and short, but you can define your variable as any name you want

2. USING THE WHILE LOOP
// In a while loop, we don't do all the steps at the same time
var variableName = startValue; 
while (variableName &lt; number) {
    // code to repeat
    
    // increase the variable
    variableName += incrementAmount;
}

// EXAMPLE: drawing a line of ellipses in the vertical direction
var y = 50;

fill(255, 0, 0); // we keep this function outside the loop because it doesn't need to be redrawn every time
while (y &lt; 325) {
    ellipse(50, y, 25, 25);
    
    y += 25;
}

3. Put as few code into the loop as possible
Try to put as little code into the loop as possible because everything in the loop has to be drawn until the loop is compelte. So to reduce lag only put the necessary code. 

4. Using continue to go to the next place in the loop;
for (var i = 0; i &lt; 5; i++) {
    if (i === 3) {
        continue; // automatically go to the next place in the loop
    } else {
        // draw code
    }
}


// 5. Nested Loops
/*A nested loop is a loop that is run inside another loop. This can create a group of things which you could imagine created a table.*/
// outer loop
fill(255, 0, 0);
for (var i = 0; i &lt; 25; i++) {
    // inner loop (each time the outer loop is run once, this who loop is executed again)
    for (var j = 0; j &lt; 25; j++) {
        // code to repeat
        rect(25, 25, 5 + (i * 10), 5 + (j * 10));
    }
}
            </pre><!--Loops-->
            <pre id="Arrays" class="code">
/**********Arrays**********/
// Arrays are variables that store multiple values in a collection.

//1. Making an array

// Step 1
var arrayName = []; // use square brackets

// Step 2 (putting values in the array)
var arrayName = [25, false, "cool", (5 > 3)]; // you can store unlimited numer of things (elements) in an array

/*As you can see, you can store numbers, booleans, boolean statements, and strings in an array; and that's not even all.*/


// 3. Accessing the values in the array

/*Arrays index start at zero; which means if we want to access the first element in the array, we'd need to use zero**/
var Number = arrayName[0];

println(Number); // prints 25

//3. Adding/removing to/from an array
There are many array methods which can do the above or variations of it, but I'll give you two of the best

// push (adding an element)
arrayName.push(value); // adds a value to the end of the array

// splice (removing an element)
arrayName.splice(index, number); // removes a "number" of elements start from the given "index"

</pre><!--Arrays-->
            <pre class="code" id="Objects">
/***********Objects***********/

/*Objects are variables that store related information about a specific thing in one collection. The difference between objects and arrays are that arrays store multiple "elements" and objects store "attributes" about one thing.*/

// 1. Making an object
var objectName = { // use curly brackets
    // attributeName : value, 
    Color : color(255, 0, 0), // Put a comma there if there is another "attribute" after this one
    x : 25,
    y : 50, // each value stored in an object is called an "attribute"
    size : 100,
    "name" : "cool thing" // we can also store "strings" as attributes for an object
};

// 2. Accessing from an object
fill(objectName.Color); // objectToAccess DOT attribute
ellipse(objectName.x, objectName.y, objectName.size, objectName.size);

// if we want to access a string attribute, we can access using array like notation;
var Message = objectName["name"];
fill(0, 0, 0);
text(Message, 25, 25);


// 3. Changing attributes from an object

/* We can treat attributes from an object like a variable, we can simply set it to whatever we want! */
objectName.size = 200; // setting the objects "size" attribute to 200

/*
**Further thought**
* Try animating an object by changing it's attribute in the draw() function, something like "objectName.x += 5;" in the draw funciton should work! 
*/
/*

            </pre><!--Objects-->
            <pre class="code" id="Object-Oriented-Design">
/***********Object-Oriented-Design (OOD)***********/
/* 
* Also known as OOP (Object-Oriented-Programming).
*
* OOD is very powerful because it lets us create methods and properties that we can reuse and change. 
* We can create "new" instances of the object constructor we made, and change it as we want.
*/

//1. Making a constructor function
var constructorName = function() {
    // we use "this" to define this object's properties
    this.x = 25;
    this.y = 50;
};

// we can create a prototype "method" to use for created instances of this object constructor
constructorName.prototype.display = function() {
    fill(0, 200, 0);
    rect(this.x, this.y, 50, 50);
};

//2. Creating "new" instances of that constructor
var newThing = new constructorName ();

//3. Using the newly created instances of that constructor
newThing.display(); // calls the prototype method which will draw a rect at the x and y position


/*
* That's not all, I'll show you a couple other things you can do!
*/
//1. Adding parameters
var objectName = function(x, y) {// adding parameters
    this.x = x; // now we are flexible; we can position the newly created instance where we want
    this.y = y;
};

// create any methods you want

// create a new instance
var newThing = new objectName (25, 25); // keep track for what the first and second arguments are!

//2. Adding more paramters
var objectName = function(config) {// adding config as a "object" paramter
    this.x = config.x;
    this.y = config.y;
};

// create any methods you want

// now when we create a new instance; we use curly brackets to symbolize we are putting an object as the parameter
var newThing = new objectName ({
    // filling in the x and y values
    x : 25, 
    y : 25
}); 


/**
* Moving on, try to do the following (ask in the Tips & Thanks if you need help);
- Create object constructor
- Create methods for it
- Create an array to store new instances of it
- use "push" to add a new instance of the constructor into that array
- then use a loop to iterate through the array and call each instance of the object's methods
**/
            </pre><!--Object Oriented Design-->
            <pre id="Images" class="code">
/**********Images**********/
/*Images are screenshots of code*/

// 1. Making an image
background(0, 0, 0, 0);// we want the background of our screenshot to be transparent
fill(255, 0, 0);
rect(0, 0, 25, 25);
// the parameters of get(x, y, width, height) symbolize the area where the picture is taken 
var Rectangle = get(0, 0, 25, 25); // we are "getting" a picture to be an image

// 2. Calling an image
// If you leave the width and height arguments empty they will be their default (what they were when the image was created)
image(ImageName, x, y, *width, *height);

// Example;
image(Rectangle, 25, 50);

/*KA has some predefined images which can get like so.*/
image(getImage(""), x, y); // simply click inside the quotation marks and choose an image

/*
For more on images you can check out this Image Tutorial; https://www.khanacademy.org/computer-programming/image-tutorial-hope/6740408654856192
*/
</pre><!--Images-->
            <pre class="code" id="Scene-Management">
/**********Scene Management********/
/* In most games or storyline programs we will need change the "scene" somehow. That is what Scene Management is; the management of changing scenes.*/

// create a variable to keep track of the current scene
var scene = "menu";


draw = function() {
    background(255, 255, 255);
    
    // display some depending on the current scene
    if (scene === "menu") {
        // draw code
        
        fill(0, 0, 0);
        text("Click to Continue", 200, 50);
    } else if (scene === "instructions") {
        // draw code
        
        fill(0, 0, 0);
        text("Click to Continue", 200, 50);
    } else if (scene === "game") {
        // draw code
    }
};

// Now need a way to change the scene
mouseClicked = function() {
    if (scene === "menu") {
        scene = "instructions";
    } else if (scene === "instructions") {
        scene = "game";
    }
};

/*
* So, we've done it; but what would be really useful is buttons; that way we could check to see if the mouse is inside of the button, and then change the scene depending on that. 

Check out this button tutorial if you're interested in using buttons;
https://www.khanacademy.org/computer-programming/button-tutorial-in-code/5843014349914112
*/
            </pre><!--Scene management-->
            <pre class="code" id="Transformations">
/**
*********Translations, Rotations, & Scaling*********
* Trransformations;
* 
* translate(x, y); // translate all the object's following this statement
* When you translate an object 50 in the x direction, instead of the object moving 50 to the right, the whole graph (all of the objects in the screen AND the screen) move 50 to the right, thus giving the appearance of the object moving 50 in the x direction (I'll explain later why this is useful).
* 
* When you rotate, the object simply rotates in that direction (positive degrees is counter-clockwise and negative degrees is clockwise). But when you rotate, you rotate with respect to the origin (0, 0), NOT the center of the object. 
* 
* scale(scaleX, scaleY); OR scale(scale);
* The scale() function multiplies all the following shapes/image/text (x/y) coordinates from the origin (0, 0) by the value(s) given. 
*
* pushMatrix(); & popMatrix(); can control the boundaries where a transformation function comes into effect; 
* pushMatrix(); translate(x, y); ... popMatrix();
*               All the code here ^^ will be moved, but after the popMatrix(); the transformations will be stopped.
* 
* Here's the trick though, most times you want an object to rotate or scale from it's center, but whenever we increase an object's x and y value, that affects how the object scales/rotates. So, here's how we can rotate and scale from an objects center.
**/

// 1. Put the objects center at the origin;
fill(0, 0, 0);
rect(-12.5, -12.5, 25, 25); // which we do by putting the object's center at the origin (half it's width and height should be out of view)

// 2. Translate the screen where you want your object to be:
pushMatrix(); 
// if we want the corner of the rectangle to be at (200, 200) we will need to translate that distance plus half the width/height (because remember, we moved it back that far to center it at the origin). 
translate(200 + 12.5, 200 + 12.5);
rotate(50);
scale(1.5);
fill(0, 0, 0);
rect(-12.5, -12.5, 25, 25);
popMatrix();
            </pre><!--Screen Changes-->
            <pre class="code" id="Sound">
/*******Sound*******/
* KA's PJS allows us to access sounds they have in their library, you do this by simply saying: 
* playSound(getSound());
* And you simply click in the parenthesis, and then scroll through their options of sound. Note that it's against the guildelines to have a sound playing as soon as the program starts.
            </pre><!--Sound-->
            <pre class="code" id="Noise">
            /**
*********Noise*********
* Perlin Noise is basically a refined version of the "random" function. Since it's more smooth and natural than the random function, it can be very useful.
* Anyway, when using the "noise()" function, instead of passing the min and max value, you pass a specific moment. The shorter the jump from two values, the more smooth the noise will be, but if you are using longer jumps for values of noise, it will be less smooth. Here's an example of variation of smoothness of noise.
* IMPORTANT NOTE: It is commonly said (& true) that PVectors are ineffecient & should not be used. A better alternative is often to make your own vector class.

draw = function() {
    background(255, 255, 255);
    stroke(0, 0, 0);
    for (var x = 0; x &lt; width; x++) {
        // As the x value of the point increases, we use noise to find a specific "y" value for that time, and multiply it times 100; the amount we multiply times "x" inside of the noise function determines how smooth it will be. For example, if we multiple it by (1/5), it will be making significantly larger jumps then what we have currently, thus making it less smooth.
        var y = noise(x/100) * 100;
        rect(x, 200 + y, 1, height - y);
    }
};

// The above is an example of 1D noise. To make 2D noise is simple enough, you simply need to use nested for loops. Here's an example of how: 
var xoff = 0.0;
for (var x = 0; x &lt; 100; x++) {
    var yoff = 0.0;
    for (var y = 0; y &lt; 100; y++) {
        // Since were dealing with 2D noise, we'll need to give two values into the noise function; then we map the vector point (giving by the noise) as the variable bright, and then we'll simply color the points based off of that variable bright
        var bright = map(noise(xoff, yoff), 0, 1, 0, 255);
        stroke(bright, bright, bright);
        point(x, y);
        yoff += 0.01;
    }
    xoff += 0.01;
}
            </pre><!--Noise-->
            <pre class="code" id="Vectors">
/**
*********(Euclidean) Vectors*********
*****How to use vectors*****
* A vector can help show us where we are, for example, if we walked 5 feet right, then 4 feet down, we would have the position (5, 4).
* In Java Script, there's an easy way to depict that; PVectors. You can use PVectors to store (x, y) values, here's an simple way to use them.
**/

//This can replace (var x = 200, y = 200;)
var position = new PVector(200, 200);
//This can replace (var xVelocity = 2, yVelocity = -2;)
var velocity = new PVector(2, -2);

var draw = function() {
    background(255, 255, 255);
    
    //Adding each individual argument of the vectors to the corresponding velocity argument
    position.add(velocity);//Note, to add a vector to another vector, you use "add" instead of "+=".
    
    // We still sometimes need to refer to the individual components of a PVector and can do so using the dot syntax: location.x, velocity.y, etc.
    if ((position.x > width) || (position.x &lt; 0)) {
        velocity.x = velocity.x * -1;
    }
    if ((position.y > height) || (position.y &lt; 0)) {
        velocity.y = velocity.y * -1;
    }
    
    noStroke();
    fill(179, 179, 179);
    ellipse(position.x, position.y, 16, 16);
};

/**
*****More vector operations*****
* Since we can't using the standard operations to add all the components of vectors another correspondings vectors components, we need some special vector operations, here's some: 
* "add()", add two vectors,
* "sub()", subtract two vectors,
* "mult()", scale two vectors with multiplication,
* "div()", scale two vectors with division,
* "mag()", calculate the magnitude of a vector,
* "normalize()", normalize the vector to a unit length of 1,
* "limit()", limit the magnitude of a vector,
* "heading2D()", the 2D heading of a vector expressed as an angle,
* "dist()", the Euclidean distance between two vectors (considered as points),
* "angleBetween()", find the angle between two vectors,
* "dot()", the dot product of two vectors,
* "cross()", the cross product of two vectors (only relevant in three dimensions),
* 
* When using vectors operations, we use the "instance" methods when increases during the program:
* vectorName.add(anotherVectorName);
* When storing vector values, we use the "static" method:
* var w = PVector.add(vectorName, anotherVectorName);
**/
            </pre><!--Vectors-->
            <pre class="code" id="Glow-Tutorial">
/**
*********How to make a glow effect*********
* It is actually really simple, all you do is use a for loop, the fourth command of stroke()/fill()/color(), and you got a glow!
**/

noStroke(); // adding a no stroke to get rid of extra lines in our glow effect
for (var Size = 25; Size &lt; 40; Size++) { // set the original "Size" as the base circle, and the max size "40" to some appropriate value for what you want
    // the four paramter of fill is alpha, which is how see-through the shape is We make the object less and less see-through as the size increases giving it a glow effect
    /** Make sure that you choose the color you want! **/
    fill(255, 0, 0, 200 - (Size * 5)); // how fast your decrease depends on what the coeffecient is on Size, in this case we use 5
    ellipse(100, 100, Size * 5, Size * 5); // we also need to decide how fast we want to increase the size of the ellipse, in this case we chose 5 as the coeffecient 
}

/* That is it, just play around with these numbers until you get what you are looking for **/




            </pre><!--Glow Tutorial-->
            <pre class="code" id="Collision-Functions">
/*********Collision Functions*********/
/**
* These notes help teach you how to create functions to check between two objects. 
**/

/** Rect To Rect Collide (RTRC) **/
var RTRC = function(rect1, rect2) {
    // returns a boolean statement; will either be true or false
    
    
    return (rect1.x + rect1.width > rect2.x  // rect1 RIGHTSIDE is greater than rect2 LEFTSIDE
         && rect1.x &lt; rect2.x + rect2.width // rect1 LEFTSIDE is less than rect2 RIGHTSIDE
         && rect1.y + rect1.height > rect2.y // rect1 BOTTOMSIDE is greater than rect2 TOPSIDE
         && rect1.y &lt; rect2.y + rect2.height); // rect1 TOPSIDE is less than rect2 BOTTOMSIDE
};

/** Rect To Ellipse Collide (RTEC) **/
var RTEC = function(ellipse, rect) {
    // NOTE: This function was made for ellipseMode(CENTER), the default for ellipses
    /**
    1. Find the closest corner of the rect to the ellipse.
    2. Calculate the distance of that corner to the center of the ellipse.
    3. Return that boolean statement.
    **/
    var closestPointX = 0, closestPointY = 0;
    
    // finding closest x side
    if (rect.x &lt; ellipse.x - ellipse.radius/2) {
        closestPointX = rect.x + rect.width;
    } else {
        closestPointX = rect.x;
    }
    
    // finding closest y side
    if (rect.y &lt; ellipse.y - ellipse.radius/2) {
        closestPointY = rect.y + rect.height;
    } else {
        closestPointY = rect.y;
    }
    
    // returns a boolean statement that checks whether or not the closest corner of the rectangle is less the ellipses radius (size)
    return pow(ellipse.x - closestPointX, 2) + pow(ellipse.y - closestPointY, 2) &lt; ellipse.radius * ellipse.radius;
};

// Defining some objects to check for
var r = {x : 25, y : 25, width : 25, height : 25};
var e = {x : 300, y : 250, radius : 50};
// an object to keep track of the mouse's coordinates
var mouse = {x : mouseX, y : mouseY, width : 0, height : 0};

draw = function() {
    background(255, 255, 255);
    // update the "mouse" object's coordinates
    mouse.x = mouseX;
    mouse.y = mouseY;
    
    // color the rectangle depending on if the mouse is colliding with it or not
    if (RTRC(r, mouse)) {
        fill(200, 0, 0);
    } else {
        fill(255, 0, 0);
    }
    rect(r.x, r.y, r.width, r.height);
    
    // color the rectangle depending on if the mouse is colliding with it or not
    if (RTEC(e, mouse)) {
        fill(200, 0, 0);
    } else {
        fill(255, 0, 0);
    }
    // since the radius of a circle is the distance from the center to any part of its side, we need to multiple the radius times 2 to get the full "width" or "height" of the circle
    ellipse(e.x, e.y, e.radius * 2, e.radius * 2);
};
            </pre><!--Collision Functions-->
            <pre class="code" id="Buttons-Using-OOD">
/*********Buttons*********/
/**
* A small tutorial teaching you how to make buttons using OOD.
* Level: Intermediate
* You'll most likely want to change your button "engine" slightly depending on your program, so you'll need to try to work that out by yourself. :)
**/

// Creating Rect and Ellipse Collision functions
/** Rect To Rect Collide (RTRC) **/
var RTRC = function(rect1, rect2) {
    // returns a boolean statement; will either be true or false
    return (rect1.x + rect1.width > rect2.x && rect1.x &lt; rect2.x + rect2.width && rect1.y + rect1.height > rect2.y && rect1.y &lt; rect2.y + rect2.height);
};

/** Rect To Ellipse Collide (RTEC) **/
var RTEC = function(ellipse, rect) {
    // NOTE: This function was made for ellipseMode(CENTER), the default for ellipses
    /**
    1. Find the closest corner of the rect to the ellipse.
    2. Calculate the distance of that corner to the center of the ellipse.
    3. Return that boolean statement.
    **/
    var closestPointX = 0, closestPointY = 0;
    
    // finding closest x side
    if (rect.x &lt; ellipse.x - ellipse.radius/2) {
        closestPointX = rect.x + rect.width;
    } else {
        closestPointX = rect.x;
    }
    
    // finding closest y side
    if (rect.y &lt; ellipse.y - ellipse.radius/2) {
        closestPointY = rect.y + rect.height;
    } else {
        closestPointY = rect.y;
    }
    
    // returns a boolean statement that checks whether or not the closest corner of the rectangle is less the ellipses radius (size)
    return abs(dist(closestPointX, closestPointY, ellipse.x, ellipse.y)) &lt; ellipse.radius;
};

var scene = "menu";

// an object to keep track of the mouse's coordinates
var mouse = {x : mouseX, y : mouseY, width : 0, height : 0};

// Creating a Button Constructor Function
var Button = function(config) { // we will define config as an object storing our needed information
    this.x = config.x;
    this.y = config.y;
    // width/height variables for rectangle
    this.width = config.width || 25;
    this.height = config.height || 25;
    // radius variable for circles
    this.radius = config.radius || 25;
    
    // is this button a circle or rectangle (ect)
    this.shape = config.shape || "rect";
    
    // two functions to contain methods for whether or not the button is being hovered over
    this.hoverEffect = config.hoverEffect || function() {};
    this.absenceHover = config.absenceHover || function() {};
    
    // creating a function to define that does something when this button is clicked
    this.clickEffect = config.clickEffect || function() {};
    
    // what is the label (title) and its size
    this.label = config.label || "";
    this.labelSize = config.labelSize || 25;
    
    // what is the color of the button
    this.color = config.color;
};

//Function to call on later to see if the mouse is inside
Button.prototype.isMouseInside = function() {
    if (this.shape === "rect") {
        return RTRC(this, mouse);
    } else if (this.shape === "circle") {
        return RTEC(this, mouse);
    }
};
    
//If the mouse is inside when we call "hover", then call "hoverEffect", else if it's not, then call "absenceHover"
Button.prototype.hover = function() {
    if (this.isMouseInside()) {
        cursor('pointer');
        this.hoverEffect();
    } else {
        cursor('auto');
        this.absenceHover();
    }
};

//If the mouse is inside when we call "click", then call the "clickEffect", (note: we only call it in the mouseClicked function, so if the mouse is inside when we click, then we call the "clickEffect"
Button.prototype.clicked = function() {
    if (this.isMouseInside()) {
        this.clickEffect();
    }
};
    
//Displaying the button
Button.prototype.display = function() {
    //Calling the hover function
    this.hover();
    fill(this.color);
    textSize(this.labelSize);
    if (this.shape === "rect") {
        rect(this.x, this.y, this.width, this.height);
        fill(0, 0, 0);
        text(this.label, this.x + this.width/2 - this.label.length * this.labelSize/3.5, this.y + this.height/2 + 5);
    } else if (this.shape === "circle") {
        // remember that the radius is only half the circle's width/height!
        ellipse(this.x, this.y, this.radius * 2, this.radius * 2);
        fill(0, 0, 0);
        text(this.label, this.x - this.label.length * this.labelSize/3.5, this.y + 5);
    }
};

// Creating a new instance of the Button Object
var button1 = new Button({
    // position and size
    x: 145, 
    y: 220, 
    radius: 50,
    label: "?",
    shape: "circle",
    // what to do when hovered over
    hoverEffect: function() {
        this.color = color(200, 0, 0);
    }, 
    // or not hovered over
    absenceHover: function() {
        this.color = color(255, 0, 0);
    },
    // what to do when clicked
    clickEffect: function() {
        scene = "scene 2"; // changing the scene
    },
});

var button2 = new Button({
    x: 50, 
    y: 50, 
    width: 75, 
    height: 50, 
    label: "back",
    hoverEffect: function() {
        this.color = color(200, 0, 0);
    }, 
    absenceHover: function() {
        this.color = color(255, 0, 0);
    },
    clickEffect: function() {
        // do something when clicked
        scene = "menu";
    },
});

// Scene Management; display the current scene
draw = function() {
    // update the "mouse" object's coordinates
    mouse.x = mouseX;
    mouse.y = mouseY;
    
    // displaying the current scene
    if (scene === "menu") {
        background(255, 255, 255);
        button1.display();
    } else if (scene === "scene 2") {
        background(200, 200, 200);
        button2.display();
    }
};

// Scene Management; Change the current scene 
mouseClicked = function() {
    // if the scene is menu check for menu buttons
    if (scene === "menu") {
        button1.clicked();
    } else if (scene === "scene 2") {
        button2.clicked();
    }
};
            </pre><!--Buttons using OOD-->
            <pre class="code" id="Pixel-Art">
/** Pixel Art **/


// A bitmap (sometimes called a bitmap array) is basically a map that maps the symbol (like "#") to something. In this case, each symbol maps to a colored rect to make our pixel art.
var bitmap = [
    "####################",
    "####################",
    "####################",
    "####################",
    "####################",
    "##########t#########",
    "#########ttt########",
    "########ttttt#######",
    "#########ttt########",
    "##########t#########",
    "####################",
    "####################",
    "####################",
    "####################"
];

// This object "palette" is our palette of colors. In here we give what color we want each symbol to represent. 
var palette = {
    // for each "#" symbol make the colorored rect black
    "#" : color(0, 0, 0),
    "t" : color(10, 89, 125)
};

// What size each of the bits art
var pixelSize = 5;

/**We are looping through the bitmap to create the pixel art**/
noStroke(); // stroke ruins pixel art
// so this loop loops through the bitmap array; meaning that we are iterating (going through) each of the "strings" in the arrays. But each "string" is composed of multiple symbols in it. So the next for loop will loop through the string to iterate through the symbols.
for (var i = 0; i &lt; bitmap.length; i++) {
    // strings work like arrays in the since that we can loop through them; each "bitmap[i]" is a string that we are looping through, starting at the index of zero (since arrays and strings start at zero)
    for (var j = 0; j &lt; bitmap[i].length; j++) {
        // 1. now, we want to fill the rect according to what the "palette" object says. So given a symbol "#" we want the color of that objects. 
        // 2. We know that the symbol will be bitmap[i][j], where the i tells what string we are in, and the j tells what index of that string we are in. But, given that symbol "bitmap[i][j]" we now need to return the palette's color of that symbol
        // 3. A sometimes forgotten way of accessing an object is using array notiation [], so we can actually access the color black if we type in "palette["#"]" which then returns the color black. 
        // 4. So, finally, let's put it all together -> palette[bitmap[i][j]] returns the wanted color, yay!
        fill(palette[bitmap[i][j]]);
        // finally, draw a rectangle in it's correct position
        // j represents how far we go in the string, so that is the "x" direction, and i is the y direction
        // we mush remember to multiply the position and size by the pixel size to!
        rect(j * pixelSize, i * pixelSize, pixelSize, pixelSize);
    }
}


/**Yay, we did it! 
* That is the basics of pixel art. Later on you will want to create a pixel art engine that let's you easily create lot's of pixel art, and maybe even play them fast to create an animation. You'll learn that later. But for now, you have a lot of fun creating pixel art ahead of you! :)
**/
            </pre><!--Pixel Art-->
            <pre class="code" id="ImageData">
/** 
********* ImagaData *********
* Imaga Data is a useful tool to color the pixels on the screen. You probably know that when it comes down to it everything is colored in pixels.
* Well, imagaData is a useful tool in PJS that we can use to effeciently color the pixels on the screen.
**/

// To use image data we must put it in the draw function.
draw = function() {
    // In many programs you will see people say "this.loadPixels" or "this.imageData" to 
    // access things about ImageData, but that is unecessary; the "this." is basically 
    // saying access this function from Processing.js but we have an auto tool that does
    // this for us.
    
    /*
    Sometimes there's a glitch in KA, where the "loadPixels" and "imageData" functions 
    don't load right away. This code checks if they've loaded, and if not, breaks out of
    the draw loop
    */
    if (!loadPixels){return;}
    
    //Declare ALL the variables we'll use (this is for performance later on)
    var p,l,x,y,w,h;
    var r,g,b;
    
    //Define them (could be done along with the declaration)
    w = width;
    h = height;
    
    // Load the pixels of the screen
    // Loads the pixel data of the current display window into the pixels[] array. This function must always be called before reading from or writing to pixels[]. Subsequent changes to the display window will not be reflected in pixels until loadPixels() is called again.
    loadPixels();
    
    //Check if "imageData" has loaded (not actually necessary right now, but could change in the future)
    if (!imageData || !imageData.data){return;}
    
    //Take "imageData" and store it in a variable
    p = imageData.data;
    
    //"p" is organized as 1D array like so:
    //[R,G,B,A, R,G,B,A, R,G,B,A...]
    //    ^        ^        ^ 
    // Pixel#1  Pixel#2  Pixel#3
    
    //R, G, B and A are Red, Green, Blue, and Alpha (aka transparency)
    
    
    //We can now make any changes to "p" we want (this is usually where the fancy math comes in)
    //You will want to squeeze every shred of performance out your code in the following loops.
    
    //To graph a simple function, we want to loop through every pixel on the screen.
    //I'll be graphing a simple gradient
    
    //Loop through every pixel by x and y
    for (x = 0; x &lt; w; x++) {
        for (y = 0; y &lt; h; y++) {
            // Set "l" to the pixel's position in "p"; same as "l = (x + y * w) &lt;&lt; 2".
            l = (x + y * w) * 4; 
            // FIRST off we multiple by 4 because image data stores pixels in a 1D array like previously shown. So every 4 pixels will be the start of coloring that specific pixel (R).
            // y * w because for every pixel y we go down we have to go another width farther into the array
            // finally we have to keep in mind how far down x we are too.
            
            // I decided to have three main variables here: "r", "g", and "b"
            // To make a gradient I'm mapping the color values off of "y"
            r = 256 - y * 0.64;
            g = 128 - y * 0.16;
            b = y * 0.32;
            
            // Setting the pixels color [r, g, b, a]
            p[l + 0] = r; // red
            p[l + 1] = g; // green
            p[l + 2] = b; // blue
            p[l + 3] = 255; // alpha; default is 255
        }
    }
    
    //At the end of processing the pixels, update them to the screen:
    // Updates the display window with the data in the pixels[] array. Use in conjunction with loadPixels(). If you're only reading pixels from the array, there's no need to call updatePixels() — updating is only necessary to apply changes.
    updatePixels();
    
    
    // In this example we are creating a static image so no need to animate
    noLoop();
};
            </pre><!--ImageData-->
        </div>
        
        <!--Ownership text-->
        <p id="owner-text"><a href="https://www.khanacademy.org/profile/ncochran2/projects" target="_blank">ncochran2</a> 2019 © <a href="https://www.khanacademy.org/computer-programming/subscribe-to-iron-studios/6260734328930304" target="_blank">IRON PROGRAMMING</a></p>
        
        <!--jQuery library-->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
        
        <!--HTML2canvas library, though I am mostly unfamiliar with this one-->
        <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/0.4.1/html2canvas.js"></script>
        
        <script>
            var searchOptions = ["lerpColor", "IIFE", "PJS-Shapes", "Text", "Variables", "Animation", "Operations", "Functions", "Conditions", "Loops", "Arrays", "Objects", "Object-Oriented-Design", "Images", "Scene-Management", "Transformations", "Sound", "Noise", "Vectors", "Collision-Functions", "Buttons-Using-OOD", "Glow-Tutorial", "Pixel-Art", "ImageData"];                 
            
        	var $Home = $("#home-page").show(), 
        	    $homeText = $(".home-hide").hide(), 
        	    $NoteBook = $("#note-page").hide(),
        	    $noteText = $(".note-hide").hide(), 
        	    $News = $("#news-page").hide(),
        	    $newsText = $(".news-hide").hide(),
                $SearchResult = $("#searchResults").hide(),
                $StorageNotes = $("#storage-notes").hide(),
                $ReadNotes = $("#read-notes").hide(),
                $Tutorial = $("#tutorials").hide(),
                $searchFalse = $("#searchFalse").hide();
        
            var currentScene = "Home", currentTutorial = "None";
            
            var MakeNotes = (function(notes) {
                var $div = $("<div>").
                    html($("#" + notes)).
                    addClass("notes").
                    addClass($("#" + notes)).
                    appendTo("#read-notes");
            });
            
            /**Making the search result buttons**/
            for (var i = 0; i < searchOptions.length; i++) {
                var $div = $("<div>").
                    text(searchOptions[i]).
                    addClass("search-results").
                    appendTo("#search-place");
            }
            
            $('.search-results').each(function(i) {
                $(this).on("click", function() {
                    currentTutorial = $(this).text();
                    MakeNotes(searchOptions[i]);
                });
            });
            
            /**Searching through the options to see if any contain a matching word**/
            var searchNum = 0;
            var Search = (function() {
                var i = 0;
                while (i < searchOptions.length) {
                    var sentence = searchOptions[i];
                    var search = $("#note-page").find("[type=text]").val();
                    
                    if (sentence.toLowerCase().indexOf(search.toLowerCase()) != -1 && search.length > 2) {
                        searchNum = 1;
                        $(".search-results").eq(i).show();
                    } else {
                        $(".search-results").eq(i).hide();
                    }
                    i++;
                }
            });
            
            /**Calling the search function when we type anything except for "ENTER"**/
            /*$("#search-bar").on("keydown", function(event) {
                if (event.keyCode == 8) {
                    searchNum = 0;
                    Search();
                } else if (event.keyCode === 13) {
                    for (var i = 0; i < searchOptions.length; i++) {
                        $(".search-results").appendTo("#searchResults");                                  
                    }
                    currentTutorial = "Processing";
                    $("body").trigger("click");
                } else {
                    searchNum = 0;
                    Search();
                }
            });*/
            
            //Hovering somewhere on the webpage
            $("body").on("mouseover", function (event) {
                var element = event.target;
                
                //Clicking on the buttons
            	if (element.matches("#home-button")) {
            	    $homeText.fadeIn();
            	} else {
            	    $homeText.hide();
            	}
            	
            	if (element.matches("#note-button")) {
            	    $noteText.fadeIn();
            	} else {
            	    $noteText.hide();
            	}
            	
            	if (element.matches("#news-button")) {
            	    $newsText.fadeIn();
            	} else {
            	    $newsText.hide();
            	}
            });
            
            //Clicking somewhere on the webpage
            $("body").on("click", function (event) {
                var element = event.target;
            	
                //Clicking on the buttons
            	if (element.matches("#home-button")) {
            	    currentScene = "Home";
            	} else if (element.matches("#note-button")) {
            	    currentScene = "Note-Book";
            	    $("#note-page").find("[type=text]").val("");
            	} else if (element.matches("#news-button")) {
            	    currentScene = "News";
            	} else if (element.matches(".back-button")) {
            	    currentTutorial = "None";
            	    $("#note-page").find("[type=text]").val("");
            	    //$(".search-results").appendTo("#search-place").hide();                    
            	    $(".notes").hide();
            	    //searchNum = 0;
            	}
            	
            	/** Searching for a tutorial **/
            	if (element.matches("#search-icon")) {
                    currentTutorial = "Processing";
                    for (var i = 0; i < searchOptions.length; i++) {
                        $(".search-results").appendTo("#searchResults");                                  
                    }
            	}
            	
            	//Hide all of the scenes
                $Home.hide();
                $NoteBook.hide();
                $News.hide();
                $ReadNotes.hide();
                $Tutorial.hide();
                $SearchResult.hide();

            	if (currentScene === "Home") {
            	    $Home.show();
            	} else if (currentScene === "Note-Book") {
            	    $NoteBook.show();
            	    if (currentTutorial === "None") {
            	        $Tutorial.show();
            	    } else if (currentTutorial === "Processing") {
            	        $SearchResult.show();
            	        if (searchNum === 0) {
            	            $searchFalse.show();
            	        } else {
            	            $searchFalse.hide();
            	        }
            	    } else {
            	        $ReadNotes.show();
            	    }
            	} else if (currentScene === "News") {
            	    $News.show();
            	}
            });
            
            var HL = {
                highlight: function(code) {
                    code = code.replace(/(\/\*[^\*][\s\S]*?\*\/)/g, '<span class="comment">$1</span>');
                    code = code.replace(/(\/\/.*?$)/gm, '<span class="comment">$1</span>');
                    code = code.replace(/(\/\*\*[\s\S]*?\*\/)/g, '<span class="important-comment">$1</span>');
                    code = code.replace(/NEW([\s\S]*?)ENDNEW/g, '<span class="new-code">$1</span>');
                    return code;
                },
                all:function(list) {
                    for (var i = 0; i < list.length; i++) {
                        list[i].innerHTML = this.highlight(list[i].innerHTML);
                    }
                }
            };
            HL.all(document.getElementsByClassName('code'));  
            
            /* CREDIT TO BLUEBIRD FOR THE AMAZING SAVE FUNCTION */
            var save = (function() {
                html2canvas(document.body,{
                    onrendered: function(canvas) {
                        b64Img = canvas.toDataURL();
                        window.top.postMessage(b64Img, "https://www.khanacademy.org/");
                    },
                    allowTaint: false,
                    useCORS: true,
                    width: 600,
                    height: 400,
                });
            });
            document.documentElement.onkeydown = (function(e) {
                if (e.keyCode === 27) {
                    save();
                }
            });
        </script>
    </body>
</html>
