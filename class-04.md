### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 4

### Notes - Chapter 4: Ch.4 “Links” (pp.74-93)

- Link to outside pages using `<a href>` tag

- You can link to internal pages using `<a href = "index.html">` instead of typing the whole address. 
  - You can also link to parent folders, child folders, etc.

- `mailto:` sends the user to their email with the "to" field completed with your choice of email

- `target="_blank"` opens a link in a new window

- Set an ID tag to an element, then link to that particular part of your site with `<a href="[whatever the id tag is]">` 
  - This is awesome! It would be cool to have the page quickly zoom to this, vs just instantly loading it
  - You can do this to a separate page by first adding that page's internal link, plus the ID tag

### Notes - Chapter 15: “Layout” (pp.358-404)

- Block-level elements all start on separate lines, like h1, p, ol
  - If a block is inside another block, then that is its containing/parent element
  - Can be *nested*

- Inline elements are things like images and font styles (bold/italics)

- Positioning schemes
  - Normal flow
    - This is the default
    - Every block appears on a separate line, dropping following elements down the page like paragraphs in a Word doc
    - They will not appear next to one another, but rather one after the other

  - Relative positioning
    - Can adjust the positioning of a particular element
  
  - Absolute positioning 
    - Positions an element depending on the box it's inside (its parent element)
    - Doesn't care what the text below it is doing, it will cover it up given the opportunity

  - Fixed positioning
    - Version of absolute positioning
    - Positions an element relative to the window, not the box it's inside
      - For example, allows you to place an element 10% down from the top of the page

  - Floating element
    - You can move the element to the far left or far right of the box it's inside
    - Text will flow around this

- Z Index
  - Changes what "layer" an element is on (you can bring it forward and back relative to other elements)

Liquid layouts look absolutely awesome, so do fixed-width layouts. Okay, so do grid layouts. They seem the most modern.

### Notes - Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)

These allow us to **organize our code**

#### Functions - Notes

Functions combine statements together so you don't have to keep reusing individual functions

Helps with code organization

**Calling a function** means you're telling a function to do its own task. 

> ...statements are not run until the function is called
  > - Jon Duckett, JavaScript & Jquery

This will be super useful if you want to refer back to, or reuse, a bit of code.

Functions need info to perform their tasks. These are called **parameters**

**Return values** are when a function gives you an answer when you ask for it

**Declaring Function Example:**

```
function userName() {
document.write('this is your username');
}
userName();
```

- All of the above is a **code block**
- Function keyword is `function`
- `userName` is function name
- the `username();` at the end is how you call the function

You can use parameters to have code do a task without knowing all the information up front. For example, you can have a function multiply height by width, then decide what numeric values height and width have later on

##### Local variables vs. Global variables

- Local can only be used within the variable and can't be accessed outside of it
  - Can reuse names
- Global can be used globally, or across your whole code, as the name implies

### Notes - Article: [“6 Reasons for Pair Programming”](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

- 2 devs working on the same computer, working on code together

- Much encouraged by Code Fellows!

- The driver is the one actually entering the info, while the navigator does the talking
  - Navigator doesn't actually enter any code, they're more "big picture" oriented

- Great way to talk out, almost wireframe, what your code should be doing

- Takes a bit more time, but produces higher quality code

- More engaging for both parties, less likely to be distracted

- Introduces you to other techniques you might not have considered

- Improves communication! Employers love this

- Preps you for job interviews, and you'll be turn-key at your new job