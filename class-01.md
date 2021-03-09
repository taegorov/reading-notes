### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 1

### Notes - HTML Chapter 1: “Structure” (pp.12-39)

- HTML structures pages kind of like a newspaper: headlines, articles, some images, etc.
- Using `<h1>` through `<h6>` you can create headings and subheadings like you would in Microsoft Word
- Structure of pages broken down into **elements**
- HTML uses *tags* like `<p>` and corresponding closing tags like `</p>`
- Can view how every other page on the internet is built using *inspect element* or *view source*
  
### Notes - HTML Chapter 8: “Extra Markup” (p.176-199)

- DOCTYPEs depend on what version of HTML you're using. We'll likely only use the following:
> `<!DOCTYPE html>`

- Add comments to your code (these won't appear on your site):
> `<!-- comment here -->` 

- Add ID attributes with:
> `<p id="id name">`

- Add class attributes with:
> `<p class="class name">`

- According to Roger Huba from Code 102, `<div>` and `<span>` elements are antiquated, but we should still know them in case we come across them from an older website

- You can add `<meta>` info on your page for Search Engine Optimization (SEO) purposes. Examples include keywords, descriptions, and page authors

- See page 194 for examples of "escape characters." This is how you add things like ampersands (&) to your page. You normally can't do this because those symbols interfere with, and are reserved for, code. For an ampersand, you'd write: `&amp;`

### Notes - HTML Chapter 17: “HTML5 Layout” (pp.428-451)

- div element used to be more important (or commonly used) before HTML5
  - articles, footers, asides (and others) no longer need \<div id\> tag
  
- HTML5 elements provide clearer code than their \<div\> cousins
  
- Headers and footers sit inside their respective elements
  
- Sidebars sit inside an \<aside\> element
  
- Content below header can sit inside a \<section\> element
  
- Styling occurs with CSS

### Notes - HTML Chapter 18: “Process & Design” (pp.452-475)

- Who is my site for?
- Why would someone want to visit? (what are they trying to achieve?)
- What info does a visitor need?
- How often will they visit?

#### Site Design Flowchart

x | - | Home | - | -
------------- | ------------- | -------------| -------------| -------------
About | Articles | Visit | Shop | Contact
History | News | Location | Merch | -
Team | News | Hours | Art | -

### Notes - JS Chapter 1: “The ABC of Programming” (pp.11-52)

**NOTE**: These notes are taken from my Code 102 course notes. I am the author of the notes, but please be aware that certain text in **block quotes** is taken from Jon Duckett's *JavaScript & JQuery* Book

> JavaScript allows you to make web pages more interactive by accessing and modifying the content and markup used in a web page while it is being viewed in a browser
 - Jon Duckett - JavaScript & JQuery

JavaScript essentially allows us to give step-by-step instructions to a browser/computer, kind of like a recipe

Allows users to interact with elements of your website, and allows your website to change depending on certain events/conditions
- e.g., if it's a certain time of day, your page might change a greeting to "good afternoon" or "good evening"

Common versions of JavaScript that you'll see on websites:
- Slideshoes
- Forms
- Forms
- Data filtration
- Reloading info on part of a page

All of the above rely on the ability to: 
> **Access** the content of a page
> 
> **Modify** the content of a page
> 
> **Program** rules or instructions the browser can follow
>
> **React** to events triggered by the user or browser

  - Jon Duckett, JavaScript & JQuery, pg 6

### Writing a Script

- What is your goal?
- What are the step-by-step instructions for completing that goal?
- Write these steps in coding language that a computer can understand

Even if scripts might appear complicated to you now, they're actually a simple set of instructions

Individual steps of a recipe might need to be broken down further. For example, when making spring rolls, "create peanut sauce" might have its own sub-instructions. *Computers need this information*

> **Vocabulary**: The words that computers understand
> 
> **Syntax** How you put those words together to create instructions computers can follow

  - Jon Duckett, JavaScript & JQuery, pg 20

Use flowcharts for the tasks you want the computer to achieve!

`<html>` is the content layer

`{css}` is the presentation layer

`javascript()` is the behavior layer

### Progressive Enhancement

All three of these layers work together to make a modern functioning website

Keeping things separate means that pages will still work if certain layers don't load/run

### Basics

- JavaScript allows you to add many features onto your webpage that change depending on a number of variables. This can range from what name someone enters into a form, the current time of day, or the changing cost of a good (among *many* others)

- JavaScript is **case sensitive**

- Calling
  
  `document.write('good afternoon');`
  - `document` = the web page
  - `.` = member operator
  - `write` = adds new text/content to your page
  - `('good afternoon')` = parameters

- JavaScript runs wherever `<script>` is added in your HTML code 

### Statements

A script is like a step-by-step instruction of how to tie your shoes (or any other set of instructions). Each step (e.g., "cross each lace") is a **statement**.

Statements end with a `;`

`{` and `}` are the start and end of a **code block**.

Each statement starts on a new line

### Comments

`/* Type comments to yourself using this structure */`

`// you can use the double forward slash for single-line comments //`

Like with HTML and CSS, these will help others understand your code better (and help you when you look back at your code months down the road)

### Variables

These are just like variables in math or logic, which are "calculated or computed"
- width and height, for example

**Declare** a variable like so:

`var quantity;`
- Where `var` is the variable keyword, and `quantity` is the variable name

Assign a value to a variable like so:

`quantity = 3;`
- `3` is the variable value
- `=` is the "assignment operator," which tells our code to assign a value to that variable.
- If the variable is not assigned a value, it is *undefined*

### Data Types
- Numeric
  - `1.35`
- String Data
  - A string of letters/numbers/characters
  - `'Good Afternoon!'`
- Boolean
  - `false` or `true` (no other options)

### Other Notes

You can multiply/add/subtract/etc. variables using just their names, provided you have provided a value (see Data Types) to your variable

##### Variable Shorthand

There are many ways to de-clutter (or simplify) creating a variable. One option is shown below:

> `var price = 5;`

instead of

> `var price;`

> `price = 5;`