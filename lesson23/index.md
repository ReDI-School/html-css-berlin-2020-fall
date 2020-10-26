---
title: Css Animations Part 2
nav_order: 23
---

# Css Animations Part 2

Let's take a look at some more css animation concepts:

-   Transforms
-   Keyframes

### The CSS Property Transform:

This handy property lets us move an element, rotate it, distort it or change the size.

Tranform types:

-   rotate
-   scale (increase / decrease size)
-   skew (distort)
-   translate (aka move across 2d / 3d planes)

We can combine these types, and do some really powerful things with it, but it means that using the property can get quite complex. Let's stick to some simple examples for now, as we we learn and practice!

```css
.elementToTransform:hover {
    transform: rotate(180deg);
}
```

```css
.elementToTransform:hover {
    transform: scale(2, 2);
}
```

```css
.elementToTransform:hover {
    transform: translateX(100px);
}
```

What do you think each of the above properties will do?

### Important Info!

-   Just like changing colors, or text decorations. transforms on their own won't 'animate'. the element will go from one state to the other, instantly.
-   We can combine these with `transitions` to go from one state to the other smoothly, like so:

```css
.elementToTransform:hover {
    transform: translateX(100px);
    transition: transform 1s ease-in-out 0.5s;
}
```

---

You might be wondering, if i can just do something like this:

```css
.elementToMakeBigger {
    height: 100px;
    width: 100px;
}
```

```css
.elementToMakeBigger:hover {
    height: 500px;
    width: 500px;
}
```

Then why bother using transform:scale()?

The answer is a little complex, and beyond the scope of our course; but basically, it's easier for the browser to change size or position using transform, than changing the height / width etc directly. This means your animations will be much smoother!

### Keyframes:

## Learn more

-   [W3Schools: Transform](https://www.w3schools.com/cssref/css3_pr_transform.asp)
