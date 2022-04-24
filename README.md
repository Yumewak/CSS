# CSS

## Inline CSS
```html
<body style="background-color: #EAF6F6;">
```

## Internal CSS
```
The following code goes inside <head>
```
```html
    <style>
        body {
            background-color:#EAF6F6;
        }

        hr {
            width: 8%;
            border-style: none;
            border-top-style: dotted;
            border-color: grey;
            border-width:6px ;
        }

    </style>
```
[Color](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)
 
[Background color](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)
 
[CSS Default Values](https://www.w3schools.com/cssref/css_default_values.asp)
 
[Border Style](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style)
 
[CSS Height](https://devdocs.io/css/height)

## External CSS
```
First we create an CSS Folder, and inside the CSS folder we create a "styles.css" file, and we put a link in the index.html
```
```html
<link rel="stylesheet" href="./CSS/styles.css">
```
```css
body {
    background-color:#EAF6F6;
}

hr {
    width: 8%;
    border-style: none;
    border-top-style: dotted;
    border-color: grey;
    border-width:6px ;
}

h1 {
    text-shadow: 1px 1px 8px #66BFBF;
    color: #66BFBF;
}

h3{
    color: #66BFBF;
    text-shadow: 1px 1px 1px #66BFBF;
}
```
[CSS Text](https://www.w3schools.com/css/css_text.asp)

## Debug CSS Code
```
You can use the Firefox or Chrome console to Debug your CSS Files

The priority is given to the inline element
1.- Inline
2.- Internal
3.- External

And what it means is that you can apply a global CSS rule to all of your web pages,
but on the individual web pages, you can apply more specific rules through using internal or inline
```

## CSS Syntax
```
Syntax refers to the grammar of the CSS language.
Just as in English, we have grammatical rules which state where you should put commas, where you should
have full stops, which words need to be capitalized.
All programming languages also have their own particular syntax.
```
```css
selector {property:value;}
h1{
    color:red;
    font-size: 200px;
}
img{
    background-color: red;
}
```
```
slector is the "who?"
property is the "what?"
value is the "how?"

So usually the best practice is to keep all of these rules in alphabetical order.
```
[CSS reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

## CSS Selectors
```
We add comment in CSS whit /* */
/*
img{
    background-color: red;
}
*/
```
```css
/*********************************TAG SELECTORS****************************/
h1{
    color:red;
    font-size: 200px;
}
/*********************************CLASS SELECTORS****************************/
.bacon {
    background-color: green;
}
```

## Classes vs Ids
```
The Id selector overrides the Tag selector
You can only have a single instance of one particular id name inside a single page.
```
```css
/*********************************ID SELECTORS****************************/
#heading{
    color:blue
}
/*********************************PSEUDE CLASS SELECTORS****************************/
img:hover{
    background-color: gold;
}
```

## Favicons
```
<link rel="icon" href="favicon.ico">
```

## Divs
```
<div>: The Content Division element
```

## Box Model
```
{height:600px;}
{width:100%;}
{border:solid;}
{border-width:50px;}
{border-top:0;}
{border-width:0px 10px 20px 30px;}

{padding:20px;}
{margin:10px;}
```
![imagen](https://user-images.githubusercontent.com/93165649/149569015-68979ee6-01ea-4f94-a141-5e9b90482ad1.png) \
[div](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div) \
[Padding](https://developer.mozilla.org/en-US/docs/Web/CSS/padding) \
[Margin](https://developer.mozilla.org/en-US/docs/Web/CSS/margin) \
[Border](https://developer.mozilla.org/en-US/docs/Web/CSS/border) \
[Border Style](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style)

## CSS Display Property
```
Display values:
Block
Inline
Inline-Block
None
```
```css
display:block;
```
```
By default some elements are what's called block display, for example <h1> and <p>
Block elements are those that take up essentially the whole width of the screen on a web page
effectively blocking out any other elements from sitting next to it on the left or on the right

Common Block Elements:
Paragraphs (<p>)
Headers (<h1> through <h6>)
Divisions (<div>)
List and list items (<ol>,<ul>,and<li>)
Forms (<form>)
```
```css
display:inline;
```
```
An inline display element only takes up as much space as it needs to in the height and in its width
With Inline Elements, you can't change the width
Common Inline Elements:
Spans (<span>)
Images(<img>)
Anchors(<a>)
```
```css
display:inline-block;
```
```
Whit inline-block display you are allowed to change its width, and also be able to make them go onto the same line
```
```css
display:none;
```
```
The none display property get rid of the element
```
```css
visibility:hidden;
```
```
Visibility can set to hidden, and what this does is that it makes that element disappear but it keeps its original 
position, and all the other elements still flow around it as if it's still there
```
[Display](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

## CSS Static and Relative Positioning
```
Rules of display
1. Content is Everything
The content is the first thing that determines how large things gets displayed and what the height and the width will be

2. Order Comes From Code
<h1></h1> <img>
<p></p>   <h1></h1>
<p></p>   <p></p>
<p></p>   <p></p>
<img>     <p></p>
The default layout order is determined by your code

3. Childern Sit On Parents
<div>
	<h1>a programmer</h1>
</div>
If inside this div you add an h1 with some text, then that h1 is going to be on top of the div so its more towards the 
viewer and away from the screen

Position property:
Static
Relative
Absolute
Fixed

Static means go along with the HTML rules and keep to the default

Relative 
selector{
	position: relative
	left: 30px;
}
This push the selector 30 pixels from the left of the previos position

Coordinates:
Top
Bottom
Left
Right

Two things tha you have to remember when you're dealing with relative positioning

The first thing is that when you move an element that has a relative position,
say we're pushing it down by 50 pixels it doesn't affect the position
of anything else on screen, it's as if the old position was kept and everything else
just flows around it as if it was never moved.

The other thing to remember is that when we change the coordinate properties,
for example we're saying make the top corner property for this relatively
positioned image 50 pixels, what that really means is that we're taking the top
of where that image used to be and we're giving it a 50 pixel Margin from the top
of our current image
```

## Fix and Absolute Positioning
```
Absolute
With absolute positioning we are positioning the element, relative to its parent
div{
position:relative
}
img {
position:absolute
right:30px;
}
in this case its parent of the img element is the div
In most cases the parent is simply the entire body of the web page
So the position when you're using absolute positioning looks liek you're givin
it a margin relative to the entire page

Fix
is positioned relative to the browser window, which means
that will stay in place even when scrolling the page
```

## Centering Elements with CSS
```css
text-align: center;
text-align:center; will center everything inside the parent element, that doesn't have a width set

margin:0 auto 0 auto;
When "auto" is applied it will center the element either vertically or horizontally
If it is a block element and it has a width set, then you're going to have to center it using this auto value in the margin
```

## Font Styling
```
First copy the code into the <head> of your html 
```
```html
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Merriweather&family=Montserrat&family=Sacramento&display=swap" rel="stylesheet"> 
</head>
```
```
Apply the CSS rules to specify families 
```
```css
h2 {
    font-family: 'Montserrat', sans-serif;
}
```

## CSS Sizing
```
Static size
```
```css
font-size: 90px;
line-height: 4;
```
```
Dynamic size
100% = 16px
1em = 16px
The value of dynamic units is inherited and added on top of whatever it got from is parent
The root em "rem" ignore all of the parent setting for the font size and just set it to the relative to the root

```
```css
font-size: 562.5%;
font-size: 5.625em
```

## Float and Clear
```
Only use float when its realy necessary
Float wrapp text around an element, leave the float property for the cases of wrapping text
Clear does the oposite
```
```css
    float: left;
    clear:right;    
```

## CSS Z-Index and stack order
```
Each element on screen has a x and y position so we can move the image up, down, lef, right, but it's also got a z position
or z-index i.e. towards you or away from you

Create 3 divs with red, yellow and blue class and give a content i.e. his respective color has content
In the css file style the divs with a 100 px height and width, and a border 1 px solid
Also style every class of red, yellow and blue with his respective background-color

One of the easy ways of making something show up on top of another thing is nesting it: put the yellow div inside the red div

Made all divs position absolute and place divs with this scheme: red at bottom, yellow in the middle, blue in front
Play with the order of divs changin the order in HTML doc

By default z-index is 0, solo changin the z-index to 1 will put the closest to the user and further away from the screen
z-index:-1 will stack at the bottom, the higher the number the closest to the user, and the lower is the number the
further away is from the user

Warning: z-index only work if your element is positioned: absolute, relative, fix

Recommend review css display, css static and relative, css fix and absolute

Hint to solve the challenge of the web page: remember that the section below is not white, it's see through by default
so you need to make the background color white explicitly if you want to cover the image
```
```html
<div class="red">Red</div>
<div class="yellow">Yellow</div>
<div class="blue">Blue</div>
```
```css
div {
    height:100px;
    width:100px;
    border:1px solid;
    position:absolute;
}
.red {
    background-color:red;
    z-index:1;
}
.yellow {
    background-color:yellow;
    top:20px;
    left:20px;
    z-index:0;
}
.blue {
    background-color:blue;
    top:40px;
    left:40px;
    z-index:-1;
}
```
```
There whas a problem with the image that in bootstrap 4, the 'col' classes have predefined 'position: relative;', in bootstrap 5, 
the col classes don't have position: relative;. So you have to add it manually to the col div by adding a custom class like
with the image being wrapped by a div and give a class i.e. <div class="image-container">, and use image-container to add position:relative
```
```css
.image-container{
    position: relative;
}
.iphone6{
    transform: rotate(25deg);
    width: 60%;
    position: absolute;
    right: 30%;
}
```
[z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)\
[rotate()](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate)

## Media query breakpoints
```
Questions:
Why so many designs for mobile and desktop?
What are media queries?
What if i only want a tag i.e. the h1 to be red under certain condition

Device:fixed thing
Browser size: can change
Viewport: size of screen

Since 2016 the number of people who browsed the web on mobiel overtook those who browsed on desktop

Options for a mobile optimization:
1.- Make a separate mobile site
2.- Make it responsive

We're going to make our web site responsive without using bootstrap, but CSS native functionality only
```
```css
@media print {
	h1 { 
		color:red;
	}
}

@media screen
@media speech
@media  <type> <feature>
```
```css
h1 {
    font-size:30px;
}
@media (min-width:900px) and (max-width:1000px) {
    h1 {
        font-size:60px;
    }
}
```
```
When we go into the tablet size or smaller we need to change the position of our image from position absolute, where it's taken
out of the HTML flow and it doesn't take up its own space, to static when it's being displayed on a smaller screen, so it starts
taking up the full amount of space that it needs again.
```
[@media](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)

## Tips and Tricks
```
You can give an id to an href of an anchor tag has a link
```
```html
<a class="nav-link" href="#footer">Contact</a>

<footer id="footer">
```
