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
