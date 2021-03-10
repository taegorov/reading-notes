### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 3

### Notes - Chapter 3: “Lists” (pp.62-73)

- Two types of lists: ordered and unordered
  
- Use `<ol>` for Ordered Lists -- these will appear like so:
1. item 1
2. item 2
3. item 3
4. and so on

- Use `<ul>` for Unordered Lists -- these will appear like so:
- item 1
- item 2
  - nested item 2.1
  - nested item 2.2

- IMPORTANT NOTE: before the lists will actually look like that, you have to add `<li>` or list items (in the examples above, the list items would be "item 1" etc.)

- Another important note: to create the nested look, you have to put another `<ol>` or `<ul>` element inside an `<li>` element

- Use `<dl>` for Definition Lists
  - `<dt>` for what is being defined
  - `<dd>` for the definition itself

### Notes - Chapter 13: “Boxes” (pp.300-329)

- Boxes from our [last reading notes](class-02.md) are set just big enough to contain their contents unless you specify otherwise
  
- Change these dimensions by a certain number of pixels (there are other units of measurement, but this is the standard)
  -  Changing by percentage means it changes by a percent of its containing box

- Use `max-width` or `min-width` to do exactly what it sounds like! Useful if you just don't want an image or text box to exceed a certain size, but otherwise vary in size
  - `min-height` and `max-height` do the same but with height

- **Overflow**! This one is cool. It changes what happens when, for example, there's too much text to fit inside a box. 
  - `overflow: hidden;` means the extra text is just hidden
  - `overflow: scroll;` will create a scrollbar

- Border/Margin/Padding:
![bordermarginpadding](https://i.stack.imgur.com/PeSIJ.gif)
> image credit: [stackoverflow.com](https://stackoverflow.com/questions/2189452/when-to-use-margin-vs-padding-in-css)

- Increasing margin and padding increases the space between text/images and other text/images

- Borders literally draw boxes around text/images and can be changed to look a number of different ways

- Use `text-align:` to change justification of the text and its corresponding box

###### Display Types

Often used for a site's nav bar

- `inline` = lines up list items (`<li>`) one next to another
- `block` = makes the `<li>` act like a block
- `inline-block` = has features of both

- Border images allow you to use custom images for your border, instead of the standard ones included in CSS

- Box shadows have several variables you can change to your liking
  - horizontal offset
  - vertical offset
  - blur distance
  - spread of shadow

- Border radius allows you to round the corners on a box

- For more complicated box shapes (that seems like an oxymoron), you can do various forms of this:
  - `border-bottom-right-radius: 10px 20px;`

### Notes - Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)

- if/else statements
  - Pretty much boils down to "*if* X is true, do Y, *else* (otherwise) do Z"
  - Useful for countless things, like if an entered password is correct, allow the user to access their banking info, otherwise (else) do some other action (like have them try to re-enter, or lock them out)

- Switch statements
  - Similar to if/else, but can be more tidy and elegant if using a lot of potential values for a variable
  - Would have been awesome to use for Lab 2 😅

- Make sure to use `===` instead of `==` because of weird quirks with JavaScript (sometimes it considers a string to be a number in an effort to be more user friendly)
  - This is called **"type coercion"**
  - There are quite a few quirks, so it's best just to avoid them and use `===`
 
-  Due to type coercion, techicallly every value in JavaScript can be true or false (or 1 or 0)
   -  Otherwise known as *truthy* and *falsy* values
   -  Things like empty strings, the number 0, and empty variables are treated as **falsy** (treated as `false`)
   -  Things like strings with content and number calculations are **truthy** (treated as `true`) 

  
#### Loops

A code block will run repeatedly (in a loop) until it returns the condition of `false`. 

`for` runs a code a certain number of times

`while` code will continue to run as long as a condition is `true`

`do...while` like `while`, with some caveats

#### Loop Counters

- Initialization
  - Create a variable and sets it to a certain number (for example, 0)

- Condition
  - Loop will continue until the counter reaches a certain number (for example <10)

- Update
  - Every time the code within curly braces is run, it changes the counter value (for example `i++` or `i--` adds or subtracts one, respectively)
