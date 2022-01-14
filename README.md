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
