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

##Centering Elements with CSS
```css
text-align: center;
text-align:center; will center everything inside will center everything inside the parent element, that doesn't have a width set

margin:0 auto 0 auto;
When "auto" is applied it will center the element either vertically or horizontally
If it is a block element and it has a width set, then you're going to have to center it using this auto value in the margin
```
