---
title: JavaScript 101
duration: "3:00"
creator:
    name: Melody Serra
    city: San Francisco
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) JavaScript 101

### LEARNING OBJECTIVES
*After this lesson, you will be able to:*

- Gain an overview of the JavaScript landscape and its placement in the web ecosystem.
- Practice programmatic thinking by writing pseudo-code.
- Write expressions that both assign and evaluate variables.
- Explain the difference between jQuery and vanilla JS.
- Register and trigger event handlers for jQuery events.  

### STUDENT PRE-WORK
*Before this lesson, you should:*

- Install Sublime Text 3 on your computer.
- Have Google Chrome on your computer.
- Complete DASH Project 1

### INSTRUCTOR PREP
*Before this lesson, instructors will need to:*

- Have the starter code ready to go to hand out to students.
- Have students install Sublime Text 3 on to computer.
- Write learning objectives on board.
- Make sure wifi network and password (GA Guest, yellowpencil) is written on board, since students will need to be online to use codepen.io.


### WORKSHOP AGENDA

| TIMING  | TYPE  | TOPIC  |
|:-:|---|---|
| 10 min  | [Opening](#opening)  | Greetings + The GA Experience  |
| 10 min  | [Introduction](#intro1)   | Web Production Workflow |
| 10 min  | [Introduction](#intro2)    | What is JavaScript?  |
| 15 min  | [Independent Practice](#ind-practice1)  | Practice Reading JavaScript |
| 5 min   | [Demo](#demo1)  | Pseudo Code|
| 15 min  | [Independent Practice](#ind-practice2)   | Thermostat |
| 10 min  | [Demo](#demo2)  | Variables and Data Types |
| 15 min  | [Guided Practice](#guided-practice1)  | Using the Console |
| 10 min  | [Demo](#demo3)  | Arithmetic Operators and Assignment Operators |
| 15 min  | [Guided/Independent Practice](#guided-practice2)  | Variables |
| 10 min  | [Demo](#demo4)  | Methods, JavaScript in Action |
| 5  min  | BREAK  |   |
| 20 min  | [Introduction](#intro3)  | jQuery, a JavaScript Library  |
| 20 min  | [Guided Practice/Independent Practice](#guided-practice3) | jQuery Codealong Part 1 |
| 10 min  | [Demo](#demo5) | jQuery Animations and Effects |
| 20 min  | [Guided/Independent Practice](#guided-practice3) | jQuery Codealong Part 2 |
| 20 min  | [Guided/Independent Practice](#guided-practice3) | jQuery + Conditionals |
| 10 min  | [Conclusion](#conclusion) | Review + Recap |
| 10 min  | [Takeaways](#takeaway) | Q&A |
---
<a name="opening"></a>
## Opening: Greetings + The GA Experience (10 min)

Did you know that there are over one billion websites that are live today? You can reach so many people by creating a website that distributes your ideas in a unique way. We'll be learning the building blocks that will allow you to get creative and bring your ideas to life.

### Review Learning Objectives

In this class, we'll gain an overview of the JavaScript landscape. We'll also get to coding some JavaScript, but before we do that, we'll have to understand how programs actually work. To do so, we'll learn what's called pseudocode, a way to write code in plain English. Doing so will allow us to focus on the logic of programs as opposed to being worried about syntax. We'll then write some basic JavaScript expressions. We'll also get into learning jQuery to add interactivity to our websites.

>Instructor Note: **You can distribute the starter code here to your class to avoid running into any issues later.**

### Peer Introductions

>Instructor Note: Ask each student to share their first name and answer the following question: "What brought you here tonight?."

***

<a name="intro1"></a>
## Introduction: Web Production Workflow (10 min)

> Instructor Note: In the following section, students will learn about the differences between front and back end languages. Discuss the topics below by dividing parts into sections. Ask students to define, explain, or recall any **specific** elements relating to the current topic, when applicable.

The process of going from an idea to a fully developed and launched site is pretty cool! Just a front-end developer can't necessarily build an entire "full-stack" website that allows for the type of functionality most clients seek today such as on a e-commerce website. A full stack developer is someone who can work on both the back-end and front-end of a website. But what exactly do those terms mean? Let's take a closer look at the web production workflow to help us understand.

![](assets/wp.jpg)

- UX: user experience, UX designers try to make it as easy as possible for people to use a webpage while achieving the purpose of the webpage.
- DesignL: designers take the wireframes created by the UX team and make them pretty (think about color palettes, font families...).
- Front End: front end developers bring the designs to life with HTML, CSS, and JS.
- Back End: back end developers give the website a "memory" with databases, authenticating users etc.

### Front End vs Back End in More Detail:

Sometimes it can be difficult to tell how the front end really differentiates from the back-end. Let's go into further detail to illustrate the difference between the two.

- Front end: everything the user can see and interact with on a site.
- Back end:  involves the database (like a virtual spreadsheet that stores data), the server (machine/computer that hosts web files), and application logic that the user does not see (such as validation of username and password entered).

We'll mostly be focusing on JavaScript as a front end language in this lesson. So let's break down the THREE front end languages are HTML, CSS, and JavaScript.

- HTML = noun (responsible for the 'things' on the page, e.g image vs paragraph)
- CSS = adjective (responsible for styles like color or font family)
- JavaScript = verb (responsible for behaviors, like drop-down menus)

### Activity

Let's go to [lyft.com](https://www.lyft.com/). When you hover over the word “Explore” in the navigation menu, we're able point out the dynamically looping hero images. You can also choose another website like [yelp.com](http://www.yelp.com/) or [airbnb.com](https://www.airbnb.com/). Answer the following question:
- Which parts of the site are front end and which is back end?

>**Check:** In summary, and in your own words, how would you describe how the front end is different from the back end of a website?


<a name="intro2"></a>
## What is JavaScript? (10 min)

So what exactly is JavaScript and what is it responsible for? To summarize, JavaScript can do a lot, including:

	- modify the behavior of content
	- create interactions and add functionality
	- animations
	- manipulating what we call the DOM

### Let's review the DOM

In order for us to understand what JavaScript is and what it is used for, we need to first understand what the DOM(Document Object Model) is. As we pointed out earlier, JavaScript is responsible for the behavior of content, interactions on the page, animations on the page and manipulating the DOM. Figuring out the DOM might sound intimidating at first, but not to worry! We've broken it down further here to illustrate how it's related to JavaScript.

The **Document Object Model(DOM)** is a collection of document nodes that are treated as objects in JavaScript. It is an object model and programming interface for HTML.

![](assets/dom.jpg)

<a name="#ind-practice1"></a>
## Independent Practice: Practice Reading JavaScript (15 min)

Let's practice reading some JavaScript using this code [codepen](http://codepen.io/nevan/pen/shtLA). Follow

Visit the codepen together and:

1. Turn to someone next to you and as a team try to figure out on a high level what is happening
2. With your partner try to make it so that the slow button changes the bulb to yellow
3. With your partner try to make it so that the go button works
4. This exercise is simply to help introduce you to what JavaScript looks like, do not get caught up in all the details just yet!

>Instructor Note: When students finish, have one or two pairs share out their understanding of what is going on and what the JavaScript is doing. Then ask another pair to share their solution to making it so that the slow button changes the bulb to yellow, and the go button works.

## Demo: Pseudo Code (5 min)

Before we start writing any Javascript, we'll learn a bit about how to write pseudocode. What is pseudocode? Well, it's a way to 'plan out' your program before coding it, which will make the coding process infinitely more seamless! To put in simple terms, it's a detailed yet readable description of what a computer program must do and it's expressed in plain english.

Take, for example, a program that lets a player know whether he or she has passed the current level. Pseudo code for this program might look like the following:

```js

passingScore = 50 points
get playerScore


if playerScore >= passingScore
    display message "Current level: Passed"
otherwise
    display message "Current level: Failed"
```

Again, the goal is to think through the problem and break it down into simple steps, which can then be written out in code. Since there are no formal rules as to how pseudo code must be written, each person's version will likely vary slightly. Indentation is often used to keep statements organized and grouped together.

> **Check**: "Why do you think it is important to plan out your program before coding it?"


## Independent Practice: Thermostat (10 min)

With a partner, write pseudo code for an application that would monitor the room temperature and adjust it so the room remains at a certain temperature.


```js
get targetTemperature
targetTemperature = 72
repeat forever

  currentTemperature = get sensor reading
  if currentTemperature < targetTemperature,
    turn on heater
  if currentTemperature >= targetTemperature,
    turn off heater
```

Instructor note:
>Instructor Note: Walk through the problem and have a couple students share what they come up with. At this point students might not have the best idea of how to name variables in the pseudocode, but that's okay! Focus on the logic here.

## Demo: Variables and Data Types (10 minutes)

Now that we've learned a bit about pseudocode and how that can help us explain JS logic, let's begin to code! The first step to learning the fundamentals of JS involves learning to tell our program to remember (store) values. This helps us use them later on!

#### Variables

The 'container' is what we use to store the value is called a **variable**. Remember these properties of a variable:
- A variable has a **name** and a **value**.
- The value can change.

To **declare** a variable, we'll use the following syntax:

```javascript
var age = 29;
```

If you want to **reassign** a variable, which means change the value of a variable, you can do the following:

```javascript
var age = 29;
age = 30;

```

> **Check**: "If we keep going with the analogy of a 'container' or 'box', why does it work this way, where you do not have to repeat the word var?"

> Answer: When you declare a variable, you create the box and you can store a value in there. When you want to swap out that value for another one, the box already exists.

#### Data Types

What can be stored in variables? There are three main data types or values that we'll want to learn about here.

**Strings**: groups of characters (either letters, numbers, or special characters like punctuation, spaces, or parentheses). They come in two varieties, 'single-quote' (also sometimes called 'string literals') and "double-quote". Though there are some differences between the two, don't worry about them for now. Strings are typically used to store text for people to read.
  Examples: ```'hello'```, ```'goodbye'```, ```'moc.liamg@gmail.com'```

**Numbers**: can be positive, negative, decimals Examples: ```20, -4.5, 300, 99.99```

**Booleans**: a data type that has a value of either ```true``` or ```false```

## Guided Practice: Using the Console (15 minutes)

We'll be using the console to practice creating variables. It's where where JavaScript is interpreted and run. You can use it to practice writing JavaScript!

1. Open up Google Chrome
2. Right click and go to "inspect"
3. Select "console"
5. Type the following:

```
console.log("Hello!");
var name = "Susan";
name;
```

```
var age = 18;
age;
```

To predict the types of data you're dealing with you can use ```typeof```.

```
typeof 3.45;
```

```
typeof true;
```

What data types did we store as the variable? That's right string and numbers. We'll learn about Booleans later in this class.


## Demo: Arithmetic Operators and Assignment Operators (10 min)

> Instructor Note: Discuss arithmetic operators and assignment operators from slides 25-26 with students.

We use operators to work with data in JavaScript. The standard arithmetic operators—which you have been learning since grade school—are supported here, including addition, subtraction, division, and so forth. Check it out:

```
2 + 4
=> 6

8 - 1
=> 7

4 / 2
=> 2

2 * 3
=> 6
```

Values are assigned using =; compound assignment statements, such as += and -=, can also be used:

```
var num = 8;
=> 8

num += 6
=> 14

num -= 6
=> 2
```

You can use ++ and -- to increment and decrement by 1, respectively. These can be used as prefix or postfix operators.

To recap, we have discussed two types of values—or, objects—that store data and offer helpful computation functions.


## Guided/Independent Practice: Variables (15 min)

> Instructor Note: Make sure your students have the starter and solution code that was distributed in the beginning of class. During this demo you will be walking students through Part 1 of the "Variables" project, starter code has been provided. **Students will complete Part 2 on their own.** Students should type in their answers directly into the ```main.js``` file and use the console to test their answers.


Find the starter code [here](variables/js/main.js)!

### Part 1
1. Declare a variable with the name "score". Assign it the value 3. (solution: var score = 3;)
2. Update the value of score. The new value should be 6. (solution: score= 6;)
3. Use console.log to print out the value of score. (solution: console.log(score);)

### Part 2

1. Declare a variable with the name "totalAmount". Assign it the value 0.
2. Update the value of totalAmount. The new value should be 10.
3. Add five to the totalAmount using the += operator.
4. Use console.log to print out the value of totalAmount.

## Demo: Methods, JavaScript in Action (10 min)

> Instructor Note: In this section you will be explaining on a high level what a JavaScript method is and how concatenation works. Go over slides 29-30.

A method in JavaScript is an action that can be performed on an object. We can make a string lowercase, uppercase or ask for the length of the string. For example, here we're making the string all lower case.


	```javascript
		var str = "Hello World";
		var res = str.toLowerCase();
		// the result of res will be:
		// hello world

	```

There are a lot more methods in JavaScript. You can find a whole list of methods and properties for strings (here)[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Methods_Index].  

We might also want to take two strings and combine or concatenate them. Concatenation simply means to take two strings and stick them together using the ```+``` operator like so!

	```javascript
		var book = "Happy";
		var summary = "Best book ever.";
		var review = book + ": " + summary;
		// Result will be: Happy: Best book ever.

	```

## Introduction: jQuery, a JavaScript Library (20 min)

jQuery is an open-source project that was released in 2006, and it's currently the most widely used JavaScript library on the web; originally, it was going to be called "JSelect", but the domain name "JSelect.com" was taken, so its creator, John Resig, decided to call it jQuery instead. jQuery allows us to query (i.e. select elements from) the DOM using the exact same selector syntax that we've used in CSS.  It makes it faster and easier to write cross-browser JavaScript and  allows us to find elements using CSS-style selectors and then do something to them using jQuery methods.

Here's some basic syntactical differences between javascript and jQuery

	```
	JS: document.getElementById('heading').innerHTML = "Your Name";

	jQuery: $('#heading').html('Your Name');

	```

jQuery is a javascript file, but before you start using jQuery, you'll need to include it in our html page. Let's download the compressed version [online](https://jquery.com/download/). Alternatively, you can link to the jQuery file in the ```<script>``` tag in your HTML like so:

```html
<head>
<script src="https://code.jquery.com/jquery-3.1.0.min.js"</script>
</head>
```

To reiterate, here are some things jQuery can do:

- jQuery can be used to manipulate the DOM. Manipulating the DOM is possible because with jQuery you can:
	- select certain elements
	- work with these elements in some way
- You select an element by doing the following:

```
$('li')     or      $('#firstParagraph')

```

The dollar sign specifies that you are using jQuery, what goes inside the parentheses and quotes is what you are selecting. As you can see, you can use your CSS-style selectors!

You manipulate or work with a certain elements. For example, ```.addClass``` is a method that you would append to the selected object. In this example you are adding a class called 'about-me'.

```
 .addClass('about-me');

```

In this example you start by selecting the h1 and then you append the method .html which will change the HTML content that is currently in between the opening and closing h1 tags.  


```
$('h1').html('Content to insert goes here');

```

## Guided/Independent Practice: jQuery Codealong (20 min)

> Instructor Note: Make sure your students have the starter code that was distributed in the beginning of class. Ask students to follow along as you complete the "Together" piece of Part 1 in the jquery_ code_along project. Take them through the workflow:

Here are the steps to get started:

	- Open the entire project folder in editor
	- Identity the script tags linking your external JavaScript file and linking the jQuery library have already been added

### Part 1 (Guided Practice)

1. Remove the highlight class from #box2 (use the ```.removeClass()``` method)

```js
$('#box2').removeClass('highlight');
```

2. Select the anchor within #box3. Change the HTML to 'jQuery!'

```js
$('#box3').find('a').html('jQuery!');
```

<a name="ind-practice"></a>

### Part 2 (Independent Practice)

> Instructor Note: This can be a pair programming activity or done independently.

Here is the prompt for the deliverable:

1. Add the ```.highlight``` class to ```#box4``` (use the ```.addClass()``` method)

2. Make the text color of the strong tag within #box2 green (use the ```.css()``` method)

**Check:** Were you able to create the desired deliverable(s)? Did it meet all necessary requirements / constraints?


## Demo: jQuery Effects and Animations (10 min)

- With jQuery you can also add effects and animations.
- Example:

```
$('h1').fadeOut(200);

```

- Additionally, with jQuery you can add what is called an **event listener**. This means that the browser is waiting for an event to occur, the event can be a mouseover or a scroll, for an action to be triggered.
- Example:

```
$('li').on('click', function() {
  // your code here
});

```

## Guided Practice/Independent Practice: Effects and Animations (10 min)

> Instructor Note: Make sure your students have the starter and solution code that was distributed in the beginning of class. Ask students to watch you as you complete the "Together" piece of Part 2 in the jquery_ code_along project. Take them through the workflow:

Here are the steps to get started:

	- Open the entire project folder in editor (if closed)
	- Type out the solution as students watch you:

1. When the anchor within #box3 is clicked
a) Slide toggle #box4
b) Fade out #box1 slowly

### Part 1 (Guided Practice)

	```js
  $('#box2').removeClass('highlight');
  ```

2. Select the anchor within #box3. Change the HTML to 'jQuery!'

```js
 	$('#box3').find('a').html('jQuery!');
```

### Part 2 (Independent Practice)

> Instructor Note: This can be a pair programming activity or done independently.

Here is a prompt for the deliverable:

 1. When the h2 is clicked on
 a) Slide up the h2
b) Add the snazzy class to the h1

> **Check:** Were students able to create the desired deliverable(s)? Did it meet all necessary requirements / constraints?

## Independent Practice: jQuery + Conditionals (20 min)

- If something is true, do one thing. If it is not, do something else. This type of logic or statement is a condition.
- Example:

```javascript
if (age > 65) {
    $('h1').html("Senior Discount Applied");

} else if (age < 18) {
    $('h1').html("Student Discount Applied");

} else {
	  $('h1').html("Sorry, you don't qualify for a discount");
}

```

<a name="conclusion"></a>
## Conclusion (10 min)
> Instructor Note:
> Review independent practice deliverable(s).
- Go over the last slides which include a discussion on who needs to know the content covered in this class. If time permits you can cover what students can do after class or you can just let them know that they can reference the last couple of slides to find out.
- Recap topic(s) covered in today's lesson.

### Takeaways: Q&A (5 min)

> There are a few listed in the slides, but feel free to remove these slides, change them, or just tell students that they are there for their reference.
