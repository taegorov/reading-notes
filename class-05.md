### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 3

### Notes - Chapter 5: “Images” (pp.94-125)

- It's good practice to keep all your images in a folder to keep you organized. In class, we've been adding "/img" to our VSC

- Add images to html with `<img>`
  - `<img src ="url">`
  - `<img alt = "desciption">`
  - `<img title = "additional info">`

- jpg, png, or gif if using rasterized images

- Use vector files when possible

- **Give credit when using images**

### Notes - Chapter 11: “Color” (pp.246-263)

##### Foreground Color

You can select colors in several ways.

- RGB values
  - `color: rgb (100.100.90);`
- Hex Codes
  - `color: #ee3e90;`
- Color Names
  - `color: DarkBlue;`
- HSLA with CSS3

##### Background Color

Useful for changing the color of **each** HTML element (body, h1, p, etc). For example:

`body {
    background-color: white;
}`

##### Understanding Color

You can use online color pickers to find specific colors you're looking for. These will show RGB Values and Hex Codes for you to add to your code (sometimes Color Names, although there are only 147 of those to pick from).

**Hue** = looks like the visible spectrum (or a rainbow)

**Saturation** = the amount of grey you want to add/remove from your color

**Brightness** = the amount of black you want to add/remove from your color

##### Contrast

**Low Contrast** is hard to read. Particularly for people with visual impairments. Stay away from this.
![low contrast](https://anchorpointegraphics.com/wp-content/uploads/2019/02/ColorContrastExamples-02.png)
 - Image credit: anchorpointegraphics.com 

**High Contrast** is much easier to read, but can be difficult to read if there is a lot of text on your page.
![high contrast](https://anchorpointegraphics.com/wp-content/uploads/2019/02/ColorContrastExamples-01.png)
 - Image credit: anchorpointegraphics.com 

**Medium Contrast** Perfect for long sections of text. Off-white text on a black (or dark) background, for example.

##### CSS3: Opacity

Allows you to change the transparency of an element and corresponding child elements. 

You can pick a value between 0.0 and 1.0

Example of 50% opacity:

`background-color: rgb(0,0,0);`

`opacity: 0.5;` 

Another method is changing the "alpha" value of an RGB Value:

`background-color: rgba(0,0,0,0.5);` note the extra a in rgb**a**

##### CSS3: HSL and HSLA

`background color: hsl(0,0%, 78%);`

First value changes Hue

Second value changes Saturation

Third value changes Lightness (essentially 'brightness', listed above)

`background color: hsla(0,100%, 100%, 0.5);`

Fourth value listed here changes Alpha (or opacity)

### Notes - Chapter 12: “Text” (pp.264-299)

- Serif vs. Sans-Serif vs. Monospace
  - Discussed in class. Serifs are the little fancy tails on some fonts, "sans serif" means without serifs, monospace means every letter is the same width (good for programming)

- Choose font with `font-family: ;`

- Choose font size with `font-size: ;`

- Align text horizontally with `text-align: '`

- Align text vertically (along an image, for example) with `vertical-align: ;`

- Indent text with `text-indent: ;`

- Add shadow to text with `text-shadow: ;`

- Stylize links (useful for nav bar) with `a:visited`, `a:hover`, `a:active`, `a:focus`

- Other attribute selectors:
  - `[=""]` targets a particular class/id
  - `[~=""]` targets things separated by a space
  - `[attr^=""]` targets things that start with a certain letter
  - `[attr*""]` targets things that contain a string of letters
  - `[attr$""]` targets things that end in a certain letter

### Notes - Blog Post JPEG vs PNG vs GIF

- Use JPG for landscapes or photographs
  
- Use PNG for images that might use transparency or sharp edge contrast
  
- Use GIF for animations
  
- PNG is largest of the 3