### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 14a

### Notes - CSS Transforms Article

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

### CSS Transitions & Animations Article


### 8 simple CSS3 transitions that will wow your users


### 6 Buttons animated


### CSS3 Animations: Keyframes

### 404

### Pure CSS Bounce Animation
