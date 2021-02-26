### Table of Contents

[Home](README.md)

[Reading Day 1](read02.md)

[Reading Day 2](day2.md)

[Read04](read04.md)

[Read05](read05.md)

[Read06a](read06a.md)

[Read08](read08.md)

# Intro + Scripts - Notes

> JavaScript allows you to make web pages more interactive by accessing and modifying the content and markup used in a web page while it is being viewed in a browser

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

# Expressions + Operators - Notes

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

There are many arithmetic operators that you might recognize from math class, but some are doubled up (like `++` or `--`). **Page 76 lists some of these operators**

# Functions - Notes

Functions combine statements together so you don't have to keep reusing individual functions

Helps with code organization

**Calling a function** means you're telling a function to do its own task. 
> ...statements are not run until the function is called

Functions need info to perform their tasks. These are called **parameters**

**Return values** are when a function gives you an answer when you ask for it

### Declaring Function Example

> `function userName() {`

>`document.write('this is your username');`

>`}`

>`userName();`

- All of the above is a **code block**
- Function keyword is `function`
- `userName` is function name
- the `username();` at the end is how you call the function

### Other Notes

You can use parameters to have code do a task without knowing all the information up front. For example, you can have a function multiply height by width, then decide what numeric values height and width have later on

