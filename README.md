# Colt Steele Web Developer Bootcamp

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

## Boilerplate code
Are sections of code that have to be included in many palces with little or no alteration. Remove verbose repetitive code.

## EM unit
An `em` is a unit equal to the currently specified font-size
```
h1 { font-size: 20px } /* 1em = 20px */
p { font-size: 16px } /* 1em = 16px */
```
The parent elements holds the initial size as 1em
```
html { font-size: 16px }
h1 { font-size: 2em } /* 16px * 2 = 32px */
```
Avoid overriding user's browser settings. Instead, initialize `html` with 100% that normally means `16px` unless the user changes default settings.
```
html { font-size: 100% } /* This means 16px by default */
```

## REM unit  
A `rem` is a unit that means **Root EM**. It's relative to the `font-size` defined in `<html>`.
```
h1 {
    font-size: 2rem;
    margin-bottom: 1rem; /* 1rem = 16px */
}
p {
    font-size: 1rem;
    margin-bottom: 1rem; /* 1rem = 16px */
}
```

## REM or EM?
Have two simple rules to start using them easy.  
https://zellwk.com/blog/rem-vs-em/
+ Size in `em` if the property scales according to it's font-size
+ Size everything else in `rem`

## Fonts
+ Google Fonts https://fonts.google.com
    + Select the fonts and features you want to include in your site and link the reference inside the `<head>` tag. It looks like this `<link href="https://fonts.googleapis.com/css?family=Noto+Serif+JP" rel="stylesheet">`

## Box model
Box model elements from inside to outside, content, padding, border and margin.
<img src="img/boxmodel-image.png" width="300" />