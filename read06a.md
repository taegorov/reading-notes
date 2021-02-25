### Table of Contents

[Home](README.md)

[Reading Day 1](read02.md)

[Reading Day 2](day2.md)

[Read04](read04.md)

[Read05](read05.md)

[Read06b](read06b.md)

[Read07](read07.md)

[Read08](read08.md)

# JavaScript & jQuery Pages 43-69 - Notes

### HTML, CSS, and JavaScript - How they Work Together

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


