### Link Home:
[Home](README.md)


### Notes - Chapter 2: “Text” (pp.40-61)

##### Structural Markup Cheatsheet:
The following need closing tags (`</p>`, for example) unless otherwise indicated

- Add headings to your page with: `<h1>` through `<h6>`

- Add standard ol' paragraphs to your page with `<p>` (alternatively, `<article>`)

- Bold with `<b>`

- Italicize with `<i>`

- Add superscript with `<sup>`

- Add subscript with `<sub>`

- Add a line break with `<br />`
  - does not need closing tag

- Add a horizontal line with `<hr />`
  - does not need closing tag
  
##### Semantic Markup Cheatsheet:
The following need closing tags (`</p>`, for example) unless otherwise indicated

These differ from structural markup because they *describe the content* vs. just adding style (like italics), although they sometimes add style (like italics) as well

- add blockquote with `<blockquote>`

- add shorter quote with `<q>`, which apparently just adds quotation marks?

- Abbreviate with `<abbr>`

- Cite with `<cite>`

- Define with `<dfn>`

- Add your contact details with `<address>`

### Notes - Chapter 10: “Introducing CSS” (pp.226-245)

- Treat every HTML element like it has an invisible box around it

- CSS allows you to change various aspects of those invisible boxes -- including making those boxes visible! (with borders)

- In the below example, `article` is the selector, `color: black;` is the declaration

`article {color: black;}`

- In the above example, `color` is the property, `black` is the value

###### External vs Internal CSS

- External links your HTML to an external .css file

- Internal styles your HTML directly in the .html file

###### Types of Selectors

There are various ways to apply styling to an element of your page. This includes Universal Selectors(`* {}`), Class Selectors (`.h1 {}`), and ID Selectors (`#stylizedh1`). 

### Notes - Chapter 2: “Basic JavaScript Instructions” (pp.53-84)

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

You can multiply/add/subtract/etc. variables using just their names, provided you have provided a value (see Data Types) to your variable

##### Variable Shorthand

There are many ways to de-clutter (or simplify) creating a variable. One option is shown below:

> `var price = 5;`

instead of

> `var price;`

> `price = 5;`

- There are many rules for naming your variables. They can't start with a number, for example. They **are case sensitive**. Their names should be descriptive, like `userCity` for the visitor's location. Make sure to use camelCase!

### Arrays

- Useful when creating a list of things that are somehow related to one another, and when you don't know how many items will belong in that list
  - do this instead of creating a bunch of variables!
  
- Example array:
>  `let familyNames;`
>
>   `familyNames = ['Tim', 'Marisa', 'Willow'];`

- Note that each value is separated by a comma
- You can have booleans, strings, and numbers inside this array! Don't have to be the same type

- The items (values) in the array act like they're in a numbered list, but **THE LIST STARTS WITH 0 INSTEAD OF 1**
  - In our example, "Tim" has an index value of 0, "Marisa" has an index value of 1, and so on
  
---
- To "access" an item in an array, use something like this:
> `let itemTwo;`
> 
> `itemTwo = familyNames[1];`

---
- To show how many items are in your list (or in your array) since you might not input that data yourself, do something like this:
> `let numNames;`
>
> `numNames = familyNames.length;`

---
### Expressions

Essentially 2 types of expressions:
1. Assign a value to a variable
2. Combine values of different variables to create another (single) variable

### Operators

Depended on by expressions

###### Assignment Operator
`color = 'red';`
- Assigns a value (`red`) to a variable (`color`)

##### Arithmetic Operator
`area = 5 * 10;`
- Does basic math, assigning `50` to the variable `area`

##### String Operator
`greeting = 'Yo' + 'Timbo';`
- Combines two strings (`Yo` and `Timbo`) to create `Yo Timbo`
- Only uses the `+` symbol

#### Comparison Operator
`Cheese = 10 > 20;`
- Compares 2 values and tells you if it's true or false. The above example would return `false`

#### Logical Operator
`Cheese = (10 > 20) && (2<8>);`
- `Cheese` now becomes `true`

There are many arithmetic operators that you might recognize from math class, but some are doubled up (like `++` or `--`). 

**Page 76 of Jon Duckett's JavaScript & JQuery lists some of these operators**

---
### Notes - Chapter 4: “Decisions and Loops” (pp.145-162)
> only up to the section on switch statements

`==` IS EQUAL TO

`!=` IS NOT EQUAL TO

`===` STRICT EQUAL TO

`!==` STRICT NOT EQUAL TO

`>` GREATER THAN

`<` LESS THAN

`>=` GREATER THAN OR EQUAL TO

`<=` LESS THAN OR EQUAL TO

---
#### Logical Operators

The below are Logical Operators:

`&&` is a **Logical And**

- Asks if 2 expressions both result in `true` 
> Tests more than one condition

`||` is a **Logical Or**
- Asks if *either* expressions result in `true`
> Tests at least one condition

`!` is a **Logical Not**
- If an expression is `true`, it changes it to `false`
> Reverses the state of an expression

---
#### Loops

A code block will run repeatedly (in a loop) until it returns the condition of `false`. 

`for` runs a code a certain number of times

`while` code will continue to run as long as a condition is `true`

`do...while` like `while`, with some caveats

---
#### Loop Counters

- Initialization
  - Create a variable and sets it to a certain number (for example, 0)

- Condition
  - Loop will continue until the counter reaches a certain number (for example <10)

- Update
  - Every time the code within curly braces is run, it changes the counter value (for example `i++` or `i--` adds or subtracts one, respectively)
