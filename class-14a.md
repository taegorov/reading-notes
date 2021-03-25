### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 14a

For today's reading, we learned a ton of cool new ways to add CSS styling to our page (or more specifically, the elements on our page). I have listed some that stood out to me below.

`transform` comes in 2D and 3D applications. It's not super well supported by browsers yet, but will be with time (as is tradition).

2D transform with `transform: scale(1.5)`. Transform will have many prefix options for browsers that might not support them.

Rotate an element with `rotate` plus a degree amount between 0 and 360. For example: 

```
transform: rotate(-25deg);
```

By default, the element rotates around its center.

Alter an element's scale with `transform: scale();`. 1 is the default value, so adding .5 in the parentheses will make it smaller, and anything greater than 1 will make it bigger.

You can scale X and Y individually with `scaleX` and `scaleY`

Slightly move (or *translate*) an element like so:

```
 transform: translateX(10px);
}
.box-2 {
  transform: translateY(5%);
}
.box-3 {
  transform: translate(10px, 5%);
}
```

Skew an element like so:

```
.box-1 {
  transform: skewX(15deg);
}
.box-2 {
  transform: skewY(-10deg);
}
.box-3 {
  transform: skew(15deg, -10deg);
}
```

You can combine the above transforms by listing them one after another. For example: 

```
transform: translateY(20px) rotate(5deg);
```

`transform-origin` changes the starting location around which an item transforms, rather than the exact center which is the default.

`perspective` seems valuable, but is not necessary. It adds a 3D "vanishing point" to 2D elements.

Z Axis can also be changed on elements, which changes their third dimension. For example, you can `rotateZ` You cannot skew an element along its Z axis.

`backface-visibility: hidden` means that an element will not show it's back side if, for example, it is rotated in a way where the back side would show. If this is not indicated, then you'll see a reverse image of the element.


> With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
>
> - https://learn.shayhowe.com/advanced-html-css/transitions-animations/

Different "states" are : `:hover`, `:focus`, `:active`, and `:target` 

A lot of the examples shown [in this article](https://learn.shayhowe.com/advanced-html-css/transitions-animations/) remind me of the transitions that I was able to apply to items using Macromedia Flash back in the day! Big time nostalgia.

Excellent example of a transition here:

```
.box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
  .box:hover {
    background: #ff7b29;
    border-radius: 50%;
  }
```

> -source: https://learn.shayhowe.com/advanced-html-css/transitions-animations/

Popular transition properties are listed in the article as well, about 1/3 of the way down the page.

`transition-delay` changes how long it takes for the transition to start occurring. 

**Super cool button example here:**

```
button {
  border: 0;
  background: #0087cc;
  border-radius: 4px;
  box-shadow: 0 5px 0 #006599;
  color: #fff;
  cursor: pointer;
  font: inherit;
  margin: 0;
  outline: 0;
  padding: 12px 20px;
  transition: all .1s linear;
}
button:active {
  box-shadow: 0 2px 0 #006599;
  transform: translateY(3px);
}
```

The rest of the readings were absolutely incredible (and *advanced*) examples of CSS application. I definitely bookmarked them!
