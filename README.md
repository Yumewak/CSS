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
