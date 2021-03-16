### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 7

### Notes - Domain Modeling

> Domain modeling is the process of creating a conceptual model in code for a specific problem
> 
> -Ryan Sobol, Sam Hamm, Keli Hansen
> 
> -https://github.com/codefellows/domain_modeling#domain-modeling 

Determine the metrics whose variables you can easily change. In the reading's example, the *popularity* of a sample video can be determined by a 1-10 rating, and a true/false value. To determine *popularity*, you just have need to factor in 2 measurable variables.
 - The *popularity* in this case is the constructor

New term: **instantiated**. 
> to call a constructor of a Class which creates an an instance or object, of the type of that Class
> 
> -[StackOverflow](https://stackoverflow.com/questions/44315657/what-is-the-exact-meaning-of-instantiate-in-java/44315687) 

`new` instantiates an object.

`this` variable initializes properties of an object -- (is this still necessary?)

This article is a perfect summary of what we did in lab today!

### Notes - Chapter 6: “Tables” (pp.126-145)

Create table wit `<table>`

`<tr>` indicates the start of each row

`<td>` represents the data in the cell

`<th>` = table heading -- **remember to add info to an empty cell** otherwise formatting will be wonky

`<td colspan="[number here]">` allows one cell to extend across multiple columns

`<td rowspan="[number here]">` allows one cell to extend across multiple rows

`<thead>` contains table headings

`<tbody>` contains the body of the table

`<tfoot>` contains the footer

**Note**: `<thead>`, `<tbody>`, and `<tfoot>` are for really long/tall tables that will display the header and footer even if a user scrolls

### Notes - Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

Objects allow you to store many pieces of data within one function. Objects can have many things like names, descriptions, heights, locations, numbers, etc. 

Create many objects like so:

```
function restaurant(name, tables, reserved) {
this.name = name;
this.tables = tables;
this.reserved = reserved;
}
```

Then add any new restaurants by doing this:

```
let timsRestaurant = new restaurant('Tim\'s Restaurant', 30, 10);
let marisasRestaurant = new restaurant(Marisa\'s Restaurant', 20, 18);
```

You can use the above information to dynamically update a web page to display the available tables at either Tim's Restaurant or Marisa's Restaurant. You'd just have the reserved subtracted from tables!

As we learned in Lab06, *arrays are objects*! They just hold many pieces of data that you can access with an index number (usually "`i`").

#### Methods of Document Object Model:

`document.write()` - simply displays text

`document.getElementById()` - returns an element

`document.querySelectorAll()` - shows a list of elements that correspond with a CSS selector

` document.createElement` - creates an element

`document.createTextNode` - creates a text node

Really helpful ways of selecting particular elements of a string (just lower case letters/just character # 5, just the very last character, delete white space, etc.) **on page 128-129** of Jon Duckett's *JavaScript & JQuery*.

An **object** is considered a "complex data type."

An **integer** = a whole number

`Math.round()` rounds to nearest integer

`Math.ceil()` rounds up to nearest integer

`Math.floor()` rounds down to nearest integer

`Math.random()` creates a random number

