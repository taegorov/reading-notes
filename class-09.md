### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 9

### Notes - HTML/CSS Book, Chapter 7: “Forms” (p.144-175)

Types of form controls

- Text
  - Text input
  
  - Password input
  
  - Text area
  
- Choices

  - Radio button

  - Checkbox

  - Drop-down box

In a form where a user inputs their username, when they click 'submit', this information gets sent to the server which is processed with PHP, C#, Java. How will we use this info?

`<input>` creates a form

`type="text"` allows for one line of text

`type="password"` creates a password entry area (hides the characters for privacy)

`name="name"` the server will need to know what has been entered (kind of like a console.log)

`maxlength` sets the max length of a text entry. Useful if you're only allowing a user to enter a year or date

`textarea` creates an expandable text entry area instead of a single line

`input type="radio"` creates a radio button

- `value=" "` sets an option

`input type="checkbox"` creates a checkbox

- `value=" "` sets an option

`select name=" "` creates a drop down list box

- `option value=" "` creates an option for the drop down box

`fieldset` groups together related forms, even adds a little box around the choices if you add `<legend>Group Details</legend>` to the top of the code!

`required="required"` shows that an entry is required


---
### Notes - HTML/CSS Book, Chapter 14: “Lists, Tables & Forms” (pp.330-357)

Bullet styles for unordered lists:

- none
  
- disc
  
- circle
  
- square

Styles for ordered lists:

- decimal (1, 2, 3)

- decimal-leading-zero (01, 02, 03)

- lower-alpha (a, b, c)

- upper-alpha (A, B, C)

- lower-roman (i. ii. iii.)

- upper-roman (I, II, III)

Use images for bullet points by adding the following to CSS:
```
ul {
    list-style-image: url("img/example.png");
}
```

`list-style-position: outside;` places the bullet point directly to the left of the text

`list-style-position: inside;` places the bullet point inside the text box, but indents the first line

#### Table properties:

- `width` changes the table width

- `padding` changes the space between the table border and the data

- `text-transform: uppercase` changes what case the entry is in

- `text-align` changes how the text is aligned in the cell

- `tr.even { background-color: grey }` changes background color of *even cells* to grey. Makes tables easier to read!

- `hover` highlights a portion of the table when your mouse hovers over it

- `empty-cells: show;` or `empty-cells: hide;` chooses whether or not to display empty cells

- `border-spacing` changes space between cells

---
### Notes - JS Book, Chapter 6: “Events” (pp.243-292)

> When you browse the web, your browser registers different types of events. It's the browsers way of saying, "Hey, this just happened." Your script can respond to these events.
> 
> -Jon Duckett, JavaScript & JQuery, page 244

Types of events (among many):

- load (page has loaded)
- error (page comes across a JS error)
- resize (window is resized)
- scroll (visitor scrolls up or down)
- keydown (button is pressed)
- click (a button is pressed)
- mouseout (mouse moves off an element)
- focus (element is in focus)
- submit (form is submitted)
- copy (content is copied in a form field)
- paste (content is pasted)

How code is triggered by an event:

(Text in quotations is taken from Jon Duckett *JavaScript & JQuery* page 249)

1. Element is decided on ("select an element")
2. An event within that element will create a response ("specify event")
3. Code that will run once that event happens ("call code")

`element.onevent` is how you attach an event to an element

`addEventListener` can recognize several functions simultaneously

#### Event Bubbling vs Event Capturing with regards to Event Flow

In *Event Bubbling* the event flows outward from a specific node to the least specific. This is the **default**.

In *Event Capturing* the event flows inward from the least specific no to the most specific.

