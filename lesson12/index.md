---
title: CSS Selectors
nav_order: 12
---

# CSS Selectors

The three most used CSS Selectors are the Element, the ID and the Class.

## The element selector selects elements based on the element name

```
h1 {
    color: #990000;
    border-bottom: #990000;
}
```

## The ID Selector uses the id attribute of an HTML element to select a specific element

- In HTML, you identify an element with an ID this way: `<h1 id="title">`
- In CSS, you refer to that ID using the hashtag: `#title`
- **Important rule**: there should be only one ID per page **with the same name**. There could be many IDs, but all of
them should have different names

```
<h1 id="title">Welcome to ReDI School</h1>

#title {
    color: #ffffff;
    border-bottom: #59ADC5;
}
```

## The class selector selects elements with a specific class attribute

- In HTML, you add a Class to an element this way: `<ul class="nobullets">`
- In CSS, you refer to that Class using a dot: `.nobullets`
- There is no limit to the number of classes per HTML file so you can have as many as you want but...if you find
yourself adding too many on one page, there's probably an easier way to do it :)

```
<ul class="nobullets">

.nobullets {
    list-style-type:none;
}
```

## You can combine IDs with Class

```
<h1 id="title" class="bigger">Welcome to ReDI School</h1>

h1 {
    font-family: sans-serif;
}
#title {
    color: #ffffff;
    border-bottom: #59ADC5;
}
.bigger {
    font-size:125%;
}
```

## IDs and Classes best practices

- Use IDs to identify main areas of a page: header, footer, content, main navigation, a photo gallery etc.
- Use classes to mark the exceptions in the code
 - For example, if you will remove the bullets from every `ul`, you don't need to apply a class to every UL, you can
 define that in the `ul`
- Take advantage of the tree structure of an HTML document: style first for the main tags and then go deeper.
 - For example, apply the text styling to `body`, so you don't have to add it to `p`, `li` or any other element.

## Nested selectors

Selectors can be nested to give you more precise control.

```
<div id="header">
    <a href="#home">Home</a>
</div>

#header a {
    color: #0066CC;
}
```

**Learn more**:

- [W3Schools: CSS Syntax and Selectors](https://www.w3schools.com/css/css_syntax.asp)
- [W3Schools: CSS Box Model](https://www.w3schools.com/css/css_boxmodel.asp)
