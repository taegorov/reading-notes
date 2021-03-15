### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 6

### Notes - Understanding The Problem Domain Is The Hardest Part Of Programming

I really liked this part:

```
Normally when you put together a jigsaw puzzle you follow steps that might look something like this:

- Figure out what the major components of the picture are
- Sort the pieces by color or component
- Put together all the border pieces
- Put together each component of the picture from the piles you created

**This all breaks down when you don’t have a picture with clear components that you can identify.**

 - John Sonmez, https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming
```

We can apply this mentality to code, where we write smaller pieces with full awareness of the bigger picture. However, the real world is not always like that. **It is much easier when we have that full awareness.**

If we have the complete specifications of the finished product, along with what our code should do when X occurs, our job is easy.

> ...understanding the problem is the most critical piece to the equation.
>  - John Sonmez, https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming

Understanding the problem makes our jobs easier!

Measure twice, cut once. Understand the actual problem before attempting to code.


### Notes - Chapter 3: “Object Literals” (pp.100-105)

> Objects group together a set of variables and functions to create a model of something you would recognize from the real world
> - Jon Duckett, JavaScript & JQuery, page 100

If a variable is in an object, it becomes a property

If a function is in an object, it becomes a method

"Literal notation" is the main way to make an object
- Example would be `name: 'Tim',`

"Dot notation"  
- Example would be `let userName = user.name;`

### Notes - Chapter 5: “Document Object Model” (pp.183-242)

Document Object Model = DOM. It is not part of HTML or JavaScript. It has its own rules. It is a "model of a webpage." (*Jon Duckett, JavaScript & JQuery, page 186*)

Also known as an **Application Programming Interface** aka API. We're getting to API's!

Made of 4 types of nodes:
1. Document Node
2. Element Node
3. Attribute Node
4. Text Node

Full breakdown of these nodes on page 186-189 of *JavaScript & JQuery*. It's worth checking out. It shows how to pick the element you want to edit.

Pages will load quicker if you're efficient with calling out elements, calling out the fewest number of nodes in order to change something.

`getElementByID()` and `querySelector()` are very similar.

NodeLists are like arrays in that their list of values start at 0.
- You can test their length with `length`
- Retrieve something from a nodelist with `item[]`

This stuff is strangely similar to the CSS selector game we had for Lab 05c.

Awesome flowchart showing looping through a NodeList shown on pages 206-207 of *JavaScript & JQuery*!

`document.write()` vs `element.innerHTML` vs DOM Manipulation
- Many advantages and disadvantages to each.

`hasAttribute()` lets you check if an attribute already exists somewhere else in your code.