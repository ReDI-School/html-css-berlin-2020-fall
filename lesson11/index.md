---
title: CSS Styling
nav_order: 11
---

# CSS Styling

## Let's style our document

CSS is very powerful and there is a lot we can do with it, but we need to start somewhere. Let's keep it simple, by
using the most common CSS properties:

### Paragraphs, headings, list items, links `<p>`, `<h1>` to `<h6>`, `<li>`, `<a>`

- `color: #FF9900;` (hex value, name, rgb, rgba)
- `text-align: left;` (center, right, justify)
- `font-size: 16px;` (px, em, rem, %)
- `font-weight: bold;` (normal, bold)
- `font-style: italic;` (normal, italic)
- `background-color: #660000;` (hex value, name, rgb, rgba)

### Box elements

Well...every element is a box, but let's focus on `<div>`, `<ul>`, `<ol>` and also the previous text elements.

- `width: 500px;` (px, em, rem, %)
- `height: 250px;` (px, em, rem)
- `border: 5px solid #CC0000;` (px, em, rem; solid, dotted, dashed; hex, name, rgb, rgba)
- `padding: 10px 20px 10px 20px;` (px, em, rem)
- `margin: 10px auto 30px auto;` (px, em, rem)

### Here is an example

```
div {
    background-color: #eeeeaa;
    padding: 16px 24px;
    margin: 32px auto;
    border: 3px solid #00cc00;
    width:50%;
}
p {
    text-align: center;
    font-size: 24px;
    font-weight: bold;
    font-style: italic;
    color: #990000;
}
```

### The Result:

<div style="background-color: #eeeeaa; padding: 16px 24px; margin: 32px auto; border: 3px solid #00cc00; width:50%;">
    <p style="text-align: center; font-size: 24px; font-weight: bold; font-style: italic; color: #990000;">Look at me, I
    know latin! Enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
Maecenas aliquet accumsan leo. Nulla quis diam. Nullam eget nisl. Praesent dapibus. Pellentesque ipsum. Mauris tincidunt
sem sed arcu. Etiam quis quam. Nullam at arcu a est sollicitudin euismod. Aenean fermentum  risus id tortor.</p>
</div>

## Let's see CSS at work

Here is the [Museum's page](./museums.html) example.

## Some sources for colors

- [Coolors.co](https://coolors.co/)
- [Color-hex.com](https://www.color-hex.com/color-palettes/)
- [Colorsupplyyy.com](https://colorsupplyyy.com/)

**Learn more**:

- [W3Schools: CSS Syntax and Selectors](https://www.w3schools.com/css/css_syntax.asp)
- [W3Schools: CSS Colors](https://www.w3schools.com/css/css_colors.asp)
- [W3Schools: CSS Box Model](https://www.w3schools.com/css/css_boxmodel.asp)

