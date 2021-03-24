### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 12

### Notes - Easily Create Stunning Animated Charts with Chart.Js 

https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/ 

Charts are way more readable than tables.

[Chart.js](https://www.chartjs.org/docs/latest/)

This resource was really straightforward and wrote out step-by-step instructions on how to add various types of graphs to my page. Animated line graphs, pie charts, and bar chart. It also included the code for how to do so.

--- 
### Notes - Basic usage of canvas

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage

`<canvas>`'s only attributes are height and width. 300px x 150px by default. If these seem distorted, edit height/width in HTML, not CSS.

Remember to add id's to `<canvas>` elements. You should also provide alt's to these!

Styling to `<canvas>` does not affect the information/styling of the drawing itself.

**Rendering Contexts** - use `getContext()`

You can literally draw with canvas/JS. Below is a screenshot of about 10 lines of JavaScript:

![image](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/228/0bed6a3ebfcc9d739a3a9fbc4de856f3/canvas_ex1.png)

> -Image credit: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage

--- 
### Notes - Drawing shapes with canvas

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes 

**Coordinate Space** - the grid we work in with canvas.

All elements are placed *relative to the top left corner of the grid*(coordinate 0, 0).

#### Ways to draw a rectangle

> fillRect(x, y, width, height)
>
>- Draws a filled rectangle.
>
>strokeRect(x, y, width, height)
>
>- Draws a rectangular outline.
>
>clearRect(x, y, width, height)
>
>- Clears the specified rectangular area, making it fully transparent. 
>
>-Source: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes

```
    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
```

The above functions are used to create this style of rectangle:

![image](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/245/abd4f1e1c012f5d3b636cd1b852b074c/Canvas_rect.png)

(*Note: the code and image above are taken from* https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)


#### Paths

You can make shapes with paths because they are points connected by lines, and can be curved or uncurved (and can be various colors).

To do so, you first create the path, then use drawing commands to draw it, then add a stroke or fill to "render" it. There are a number of functions that do this:

> `beginPath()` Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

>`Path methods` Methods to set different paths for objects.

>`closePath()` Adds a straight line to the path, going to the start of the current sub-path.

>`stroke()` Draws the shape by stroking its outline.

>`fill()` Draws a solid shape by filling the path's content area. 

>`moveTo(x, y)` Moves the pen to the coordinates specified by x and y. 

(*Note: the definitions above are taken from* https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

---

### Notes - Applying styles and colors

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors 
`
> `fillStyle = color` Sets the style used when filling shapes.

> `strokeStyle = color` Sets the style for shapes' outlines. 

(*Note: the definitions above are taken from* https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors )

Colors are set to black by default. Once you select a new color using the code above, those will become the default for whatever you draw from then on.

7 lines of JavaScript (using for loops!) can result in this:

![image](https://media.prod.mdn.mozit.cloud/attachments/2013/06/24/5417/e352ec307d004a83b2df969b9f33539f/Canvas_fillstyle.png)

> -Image credit: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors 

You can use `strokeStyle` instead of `fillStyle` to create lines, and `arc` to create circles.

This page also has some great ways to change the Line Style of your drawing, including `lineCap`s, which can be `square`, `round`, or `butt`. 

`lineJoin` determines how lines are connected to one another.

This example taken from the reading (https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors) is mindblowing:

![image](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/222/bcf90d24adf679755d47e6e2adf31afa/Canvas_createpattern.png)

---

### Drawing text

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text 

`fillText` vs `strokeText` are similar concepts to `strokeStyle` and `fillStyle`. `strokeText` shows text with only its outline. This actually didn't work using Mozilla Firefox, but it worked with Chrome. Which is funny considering the source.

Various 

> `font = value` current style of text.

> `textAlign = value` start, end, left, right or center. The default value is start.

> `textBaseline = value` top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

> `direction = value` Directionality. Possible values: ltr, rtl, inherit. The default value is inherit. 

![image](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text/baselines.png)

(*Note: the image and slightly reworded definitions above from* https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)