---
title: JavaScript 101
duration: "2:00"
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

- Have students install Sublime Text 3 on to computer.
- Write learning objectives on board.
- Make sure wifi network and password (GA Guest, yellowpencil) is written on board, since students will need to be online to use codepen.io.

---
<a name="opening"></a>
## Opening (10 mins)

- Review current lesson objectives.

> You can then include a hook / real-world relevance, here is a suggestion:
	 "Did you know that there are over one billion websites that are live today? You can reach so many people by creating a website that distributes your ideas in a unique way. We'll be learning the building blocks that will allow you to get creative and bring your ideas to life."

- Each student will share first name and answer the following question: "What brought you here tonight?."

***

<a name="introduction"></a>
## Introduction (10 mins)

> Instructor Note: In the following section, students will learn about the differences between front and back end languages. Discuss the topics below by dividing parts into sections. Ask students to define, explain, or recall any **specific** elements relating to the current topic, when applicable.


#### Web Production Workflow:

![](assets/wp.jpg)

The process of going from an idea to a fully developed and launched site is pretty cool! Just a front-end developer can't necessarily build an entire "full-stack" website that allows for the type of functionality most clients seek today such as on a e-commerce website. A full stack developer is someone who can work on both the back-end and front-end of a website. But what exactly do those terms mean? Let's take a closer look at the web production workflow to help us understand.

- UX - user experience, UX designers try to make it as easy as possible for people to use a webpage while achieving the purpose of the webpage.
- Design - designers take the wireframes created by the UX team and make them pretty (think about color palettes, font families...).
- Front End - front end developers bring the designs to life with HTML, CSS, and JS.
- Back End - back end developers give the website a "memory" with databases, authenticating users etc.

#### Front End vs Back End in More Detail:

Sometimes it can be difficult to tell how the front end really differentiates from the back-end. Let's go into further detail to illustrate the difference between the two.

- Front end: everything the user can see and interact with on a site.
- Back end:  involves the database (like a virtual spreadsheet that stores data), the server (machine/computer that hosts web files), and application logic that the user does not see (such as validation of username and password entered).

We'll mostly be focusing on JavaScript as a front end language in this lesson. So let's break down the THREE front end languages are HTML, CSS, and JavaScript.

	- HTML = noun (responsible for the 'things' on the page, e.g image vs paragraph)
	- CSS = adjective (responsible for styles like color or font family)
	- JavaScript = verb (responsible for behaviors, like drop-down menus)

Let's go to [lyft.com](https://www.lyft.com/). When you hover over the word “Explore” in the navigation menu, we're able point out the dynamically looping hero images. You can also choose another website like [yelp.com](http://www.yelp.com/) or [airbnb.com](https://www.airbnb.com/).

> Instructor Note: If time permits you can visit like expedia.com and describe to students which part of the site is front end and which is back end.

> **Check:** In summary, and in your own words, how would you describe how the front end is different from the back end of a website?


## What is JavaScript? (15 mins)

In order for us to understand what JavaScript is and what it is used for, we need to first understand what the DOM(Document Object Model) is. As we pointed out earlier, JavaScript is responsible for, the behavior of content, interactions on the page, animations on the page and manipulating the DOM. Figuring out the DOM might sound intimidating at first, but not to worry! We've broken it down further here to illustrate how it's related to JavaScript.

The **Document Object Model(DOM)** is a collection of document nodes that are treated as objects in JavaScript. It is an object model and programming interface for HTML.

Let's practice reading some JavaScript in this PRACTICE READING JS using this [codepen](http://codepen.io/nevan/pen/shtLA). The directions in the slide read as follows:

Visit this  codepen together
1. Turn to someone next to you and as a team try to figure out on a high level what is happening
2. With your partner try to make it so that the slow button changes the bulb to yellow
3. With your partner try to make it so that the go button works
4. This exercise is simply to help introduce you to what JavaScript looks like, do not get caught up in all the details just yet
>
>Instructor Note: When students finish, have one or two pairs share out their understanding of what is going on and what the JavaScript is doing. Then ask another pair to share their solution to making it so that the slow button changes the bulb to yellow, and the go button works.

## Intro to Pseudo Code (10 mins)

Before we start writing any JavScript, we'll learn a bit about how to write pseudocode. What is pseudocode? Well, it's a way to 'plan out' your program before coding it, which will make the coding process infinitely more seamless! To put in simple terms, it's a detailed yet readable description of what a computer program must do and it's expressed in plain english.

> **Check**: "Why do you think it is important to plan out your program before coding it?"

## Coding JavScript: Variables (15 minutes)

Now that we've learned a bit about pseudocode and how that can help us explain JS logic, let's begin to code! The first step to learning the fundamentals of JS involves learning to tell our program to remember (store) values. This helps us use them later on!

The 'container' we use to store the value is called a variable.
- A variable has a name and a value.
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
>
> Answer: When you declare a variable, you create the box and you can store a value in there. When you want to swap out that value for another one, the box already exists.
>

- What can be stored in variables?
	- Strings: letters and other characters enclosed in quotes
	- Numbers: can be positive, negative, decimals
	- Booleans: either true or false

> Discuss arithmetic operators and assignment operators from slides 25-26 with students.
>
> At this point in the class, introduce what the "console" is and what it is used for. Model for students how to get to the console:
>
> 	1. Open up Google Chrome
> 	2. Right click and go to "inspect"
> 	3. Select "console"
> 	4. Explain that this is a place where JavaScript is interpreted and run. You can use it to practice writing JavaScript
> 	5. Type:
>
> 		console.log("Hello!");
>
> 		 var name = "Susan";
>
> 		name;
> 	6. Ask students "What data type did we store as the variable?"

## Demo: Variables (10 mins)

> During this demo you will be walking students through Part 1 of the "Variables" project, starter code has been provided. Part 1 instructions state:
>
> 1. Declare a variable with the name "score". Assign it the value 3. (solution: var score = 3;)
> 2. Update the value of score. The new value should be 6. (solution: score= 6;)
> 3. Use console.log to print out the value of score. (solution: console.log(score);)

> Students will complete Part 2 on their own. The instructions are:
>
> 1. Declare a variable with the name "totalAmount". Assign it the value 0.
> 2. Update the value of totalAmount. The new value should be 10.
> 3. Add five to the totalAmount using the += operator.
> 4. Use console.log to print out the value of totalAmount.

## JavaScript in Action (10 mins)

> In this section you will be explaining on a high level what a JavaScript method is and how concatenation works. Go over slides 29-30.
>

- JavaScript method: ac action that can be performed on an object.
	- Example:

	```javascript
		var str = "Hello World";
		var res = str.toLowerCase();
		// the result of res will be:
		// hello world

	```

- Concatenation: to take two strings and stick them together using the + operator.

- Example:

	```javascript
		var book = "Happy";
		var summary = "Best book ever.";
		var review = book + ": " + summary;
		// Result will be: Happy: Best book ever.

	```

## How is jQuery different from JavaScript? (5 mins)

- jQuery:
	- jQuery is a JavaScript file you include in your pages.
	- makes it faster and easier to write cross-browser JavaScript.
	- allows us to find elements using CSS-style selectors and then do something to them using jQuery methods.

	```
	JS: document.getElementById('heading').innerHTML = "Your Name";

	jQuery: $('#heading').html('Your Name');

	```

## How does jQuery work? (15 mins)

- jQuery can be used to manipulate the DOM.
- Manipulating the DOM is possible because with jQuery you can:
	- select certain elements
	- work with these elements in some way
- You select an element by doing the following:

```
$('li')     or      $('#firstParagraph')

```

- The dollar sign specifies that you are using jQuery, what goes inside the parentheses and quotes is what you are selecting. As you can see, you can use your CSS-style selectors!
- You manipulate or work with a certain element by doing the following:

```
 .addClass('about-me');

```

- .addClass is a method that you would append to the selected object. In this example you are adding a class called 'about-me'.

- With jQuery you can do something like this:

```
$('h1').html('Content to insert goes here');

```

- In this example you start by selecting the h1 and then you append the method .html which will change the HTML content that is currently in between the opening and closing h1 tags.  

***

> Ask students to watch you as you complete the "Together" piece of Part 1 in the jquery_ code_along project. Take them through the workflow:
>
	- Clone the project from GitHub
	- Open the entire project folder in editor
	- Point out that the script tags linking your external JavaScript file and linking the jQuery library have already been added
	- Type out the solution as students watch you:
>
> // 1. Remove the highlight class from #box2 (use the .removeClass() method)
>
$('#box2').removeClass('highlight');
>
>// 2. Select the anchor within #box3. Change the HTML to 'jQuery!'
>
$('#box3').find('a').html('jQuery!');

<a name="ind-practice"></a>
## Independent Practice: jquery _code _along (5 mins)


> Instructor Note: This can be a pair programming activity or done independently.

Here is the prompt for the deliverable:

Part 1 - Now you try:

// 1. Add the .highlight class to #box4 (use the .addClass() method)

// 2. Make the text color of the strong tag within #box2 green (use the .css() method)


**Check:** Were students able to create the desired deliverable(s)? Did it meet all necessary requirements / constraints?

***

## How does jQuery work? (10 mins)

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

> Ask students to watch you as you complete the "Together" piece of Part 2 in the jquery_ code_along project. Take them through the workflow:
>
	- Open the entire project folder in editor (if closed)
	- Type out the solution as students watch you:
>
> 	// 1. When the anchor within #box3 is clicked
>
	// a) Slide toggle #box4
>
	// b) Fade out #box1 slowly
>
	$('#box2').removeClass('highlight');
>
>	// 2. Select the anchor within #box3. Change the HTML to 'jQuery!'
>
>```
> 	$('#box3').find('a').html('jQuery!');
```


<a name="ind-practice"></a>
## Independent Practice: jquery _code _along (5 mins)



> Instructor Note: This can be a pair programming activity or done independently.

Here is a prompt for the deliverable:

Part 2 - Now you try:

// 2. When the h2 is clicked on

// a) Slide up the h2

// b) Add the snazzy class to the h1


> **Check:** Were students able to create the desired deliverable(s)? Did it meet all necessary requirements / constraints?

***

## Conditionals (10 mins)

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

## Conclusion (10 mins)
>
- Review independent practice deliverable(s).
- Go over the last slides which include a discussion on who needs to know the content covered in this class. If time permits you can cover what students can do after class or you can just let them know that they can reference the last couple of slides to find out.
- Recap topic(s) covered in today's lesson.

***

### BEFORE NEXT CLASS
|   |   |
|---|---|
| **HOMEWORK** | Dash Project 4 and 5  |


### ADDITIONAL RESOURCES
>
>- Add your own resources.
- There are a few listed in the slides, but feel free to remove these slides, change them, or just tell students that they are there for their reference.
