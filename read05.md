### Table of Contents

[Home](README.md)

[Reading Day 1](read02.md)

[Reading Day 2](day2.md)

[Read04](read04.md)

[Read06a](read06a.md)

[Read06b](read06b.md)

# Chapter 11: Color - Notes

### Foreground Color

You can select colors in several ways.

- RGB values
  - `color: rgb (100.100.90);`
- Hex Codes
  - `color: #ee3e90;`
- Color Names
  - `color: DarkBlue;`
- HSLA with CSS3

### Background Color

Useful for changing the color of **each** HTML element (body, h1, p, etc). For example:

`body {
    background-color: white;
}`

### Understanding Color

You can use online color pickers to find specific colors you're looking for. These will show RGB Values and Hex Codes for you to add to your code (sometimes Color Names, although there are only 147 of those to pick from).

**Hue** = looks like the visible spectrum (or a rainbow)

**Saturation** = the amount of grey you want to add/remove from your color

**Brightness** = the amount of black you want to add/remove from your color

### Contrast

**Low Contrast** is hard to read. Particularly for people with visual impairments. Stay away from this.
![low contrast](https://anchorpointegraphics.com/wp-content/uploads/2019/02/ColorContrastExamples-02.png)

**High Contrast** is much easier to read, but can be difficult to read if there is a lot of text on your page.
![high contrast](https://anchorpointegraphics.com/wp-content/uploads/2019/02/ColorContrastExamples-01.png)

**Medium Contrast** Perfect for long sections of text. Off-white text on a black (or dark) background, for example.

### CSS3: Opacity

Allows you to change the transparency of an element and corresponding child elements. 

You can pick a value between 0.0 and 1.0

Example of 50% opacity:

`background-color: rgb(0,0,0);`

`opacity: 0.5;` 

Another method is changing the "alpha" value of an RGB Value:

`background-color: rgba(0,0,0,0.5);` note the extra a in rgb**a**

### CSS3: HSL and HSLA

`background color: hsl(0,0%, 78%);`

First value changes Hue

Second value changes Saturation

Third value changes Lightness (essentially 'brightness', listed above)

`background color: hsla(0,100%, 100%, 0.5);`

Fourth value listed here changes Alpha (or opacity)
