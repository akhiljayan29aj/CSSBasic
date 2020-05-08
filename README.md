# HOW TO USE THIS CSS SANDBOX

Just go through the above codes serial wise and refer this readme section for notes. I am using Visual Studio Code as my editor.

###### NOTE: If any of the styles or images are not loading you may check the path link as it may have changed when I uploaded the files.

## 01. Basics Implementation

- Inline CSS
```
<h1 style="color: red">Heading One</h1>
```
This method uses the "style" attribute. This is harder to read and change therefore not reccomended.

- Internal CSS
```
<style>
    /* This is a CSS comment */
    /* Internal CSS */
    h2{
      color: green;
    }
  </style>
```
This method uses the style tag which is placed in the head tag.

This is the syntax for a CSS code
![CSS Syntax](https://www.w3schools.com/css/selector.gif)

- External CSS

In this method we make a seperate '.css' file and link it to the html file.

We use a link tag in the head tag to link the '.css' file.

```
<link rel="stylesheet" href="/css/01_style.css">
```

## 02. Selectors

- Element selector
```
body{
  background-color: #333;
}
```
Elements can be easily selected by using their name as selector.

- Class selector
```
.primary-heading{
  color: green;
}
```
The classes can be selected using "." before the name of the class.

- ID selector
```
#welcome{
  background-color: #f4f4f4;
}
```
The IDs can be selected using "#" before the name of the ID.

- Multiple selectors
```
#welcome, #about {
  border: 1px solid #ccc;
  padding: 10px;
  margin-bottom: 5px;
}
```
We can select multiple selectors at one time just by simply using a comma "," .

- Nested selector
```
#welcome p{
  font-size: 20px;
}
```
We can target a specific element by nesting. Just use space after a parent element and then put the child you want to select.

## 03. Fonts

We usually  use the font on the body selector for consistency in the page.
```
body{font-family: Arial, Helvetica, sans-serif;}
```
This is a font stack. This stack usually contains 3-4 fonts. The first font takes priority, if it is not available for some reason the next font in the stack is used.

Web Safe Fonts: Some fonts are not available on the browser so we can include web safe fonts in the stylesheet. I use [Google Fonts](https://fonts.google.com/).

[How to use Google Fonts](https://www.freecodecamp.org/news/how-to-use-google-fonts-in-your-next-web-design-project-e1ad48f1adfa/)

```
body{
  font-size: 18px;
  line-height: 1.6em;
}
```
"font-size" property is used to set the size of the font. The default provided by the HTML tag is 16px.

"line-height" property is used to set distance between the lines.

###### CSS Absolute Units
cm(centimeter), mm(milimeter), in(inch), px(pixels, most common, is equal to 1/96 of an in), pt(points, used in word, is equal to 1/72 of an in) and pc(picas picas).

###### CSS Relative Units
%(percentage of the parent element), em(multiplier to the font size of the parent element), rem(multiplier to the font size of the root element).

```
span{font-weight: bold;
     font-style: italic;}
```
"font-weight" property is used for boldness of the text.

"font-style" property is used for styling of the text. We can use different stylings.


















