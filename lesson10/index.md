---
title: Intro to CSS
nav_order: 10
---

# Intro to CSS

## What is CSS?

CSS stands for Cascading Style Sheet. It describes how HTML elements are to be displayed on different screens and in print. It works on top of the HTML and makes use of the tree-structure of the HTML documents. The HTML elements inherit stylistic properties through CSS.

### How do we write CSS?

Here's a sintax example of a CSS rule:

```
selector {
    property: value;
}
```

### How does it work?

- The selector points to the HTML element you want to style
- The declaration block contains one or more declarations separated by semicolons.
- Each declaration includes a CSS property name and a value, separated by a colon.
- A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.

```
h4 {
    color: #0066CC;
    font-style: italic;
}
```

<h4 style="color: #0066CC; font-style: italic;">This is how the h4 with #0066CC color and italic font style it looks.</h4>

## Let's see CSS at work

Here is the [Museum's page](./museums.html) example. Let's do some really basic styling.

## The box model

All HTML elements can be considered as boxes. In CSS, the term "box model" is used when talking about design and layout.

The CSS box model is essentially a box that wraps around every HTML element. It consists of margins, borders, padding, and the actual content.


- **Content**: The content of the box, where text and images appear
- **Padding**: Clears an area around the content. The padding is transparent
- **Border**: A border that goes around the padding and content
- **Margin**: Clears an area outside the border. The margin is transparent

## CSS most used properties

| Property            |  Values                                                | Used with Elements                          |
| ------------------- | ------------------------------------------------------ | --------------------------------------------|
| color               | #RRGGBB (Red, Green, Blue hex values)                  | any element that contains text              |
| text-align          | left \| right \| center \| justify                     | block elements `h1`...`h6`, `p`, `li`, etc. |
| text-decoration     | none \| underline \| overline \| line-through \| blink | mostly with a (anchor) elements             |
| text-transformation | none \| capitalize \| uppercase \| lowercase           | any element that contains text              |
| line-height         | % or em/rem/px                                         | block elements `h1`...`h6`, `p`, `li`, etc. |
| letter-spacing      | normal or em/rem/px value                              | any element that contains text              |
| font-family         | font or font-family [, font or font-family ...]        | any element that contains text              |
| font-size           | em/rem/px value                                        | any element that contains text              |
| font-style          | normal \| italic \| oblique                            | any element that contains text              |
| font-weight         | normal \| bold                                         | any element that contains text              |

