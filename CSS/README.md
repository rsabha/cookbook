# CSS help

this will include .scss for rails, and also html.

### References

selectors: `.class, #id, HTML element`

properties: `color:, text-align:, background-color:`

### HTML elements

you can style a single element, or they can be grouped.

```
p { }
p, h1, h2 { }
```

the `body` element will wrap all content you can see on the page
so its useful if you would like to change the page `background-color`.

`footer` useful.

### CSS properties

`color` - color of text

`background-color` - background div, button, etc

`font-size` - in px (font-weight: is to make bold)

`margin` - `margin: 10px;` or  `margin: top right bottom left;`

`padding`- `padding: 10px;` or  `padding: top right bottom left;`

note: padding creates extra space within an element, while margin creates extra space around an element.

`text-align:` - aligns only text within an element

`justify-content:` (used in conjution with `display: flex`) "The justify-content property aligns the flexible
container's items when the items do not use all available space on the
main-axis (horizontally)."

[property reference doc](https://www.w3schools.com/cssref/default.asp)


### rails & .scss 

`assets/stylesheets/application.scss` - global css file: all id's
and classes defined here should be accessable by all `views/*.erb`
files.

variables are possible in `.scss` files:

```
$background-color: #544a56;

body {
  background-color: $background-color;
}

button {
 background-color: $background-color;
}
```

### class & id

`<div id="links">`:

- define in .scss file like `#content {...`

`<div class="article green">`

- define in .scss file like `.content {...`

id's can only be referenced once per page, by an element. and may only contain a single
 id, not like a class where you can have mutiple: `class="article
green"`. besides css they also have a special function that can
be used. example:

```
<body>
<a href="#article">article</a>
...9000 lines of code later...
<h2 id="article">
</body>
```

if you access that page in your browser and click on the article link,
then the browser will automatically scoll you down to the position of
the h2 title.

