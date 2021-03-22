### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 11

### Notes - HTML Book - Chapter 16: “Images” (pp.406-427)
> Controlling the size and alignment of your images using CSS keeps rules that affect the presentation of your page in the CSS and out of the HTML markup.
>
> -Jon Duckett, *HTML & CSS*, page 407

`width:` affects width.

`height:` affects height.

`float: left` and `float: right` align images to the left and right, respectively. Text will appear on the sides of these images.

Center an image by turning it into a `block` element, then `margin: 0px auto;`.

Add a background image with `background-image: url("img/example.jpg");`.

Repeat an image with `repeat`. For a background image this would be `background-repeat`. You can also specify whether it repeats on the X axis or Y axis with `repeat-x` and `repeat-y`. 

`Background-position` sets the position of a background image if it is not repeated. 

`:hover` and `:active` affect how an image looks when your mouse rolls over it. 


### Notes - HTML Book - Chapter 19: “Practical Information” (476-492)

SEO - Search Engine Optimization

- On-page techniques are things *you* can do to increase your "Google score" (vs. other things more out of your control, like how many other pages link to your site).

Add keywords wherever it makes sense! Don't try to trick the system by adding invisible keywords or anything, otherwise you'll be penalized.

A good way to get keywords on your site is to brainstorm. Think of various terms someone who'd be interested in your site might plug into Google. There are also tools online that are like keyword thesauruses.

Google Analytics is about as important as I thought it would be. You should create an account ASAP! You add their tracking code before the `</head>` tag.

Visits vs. Unique Visits - important distinction if you want new visitors to your site.

Bounce Rate = when people leave your site on the same page they arrived on. It suggests that people don't stay on your site for very long and don't find the info they need.

SQL and ASP.Net are "server-side languages and databases" (Jon Duckett, *HTML & CSS*, page 488)

FTP = File Transfer Protocol

### Notes - MDN article on audio and video elements

> The `<video>` and `<audio>` elements allow us to embed video and audio into web pages.
> 
> - https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs

Holy cow, this website's example Repo has 780 commits and 97 contributors!

All of the elements of the video player require their own variable names (constants in this case). 9 total, including 1 for pause and 1 for stop.

"Play" (and other functions) will require an event listener. Seems pretty obvious in hindsight, but cool to learn.