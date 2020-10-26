---
title: Css Animations
nav_order: 22
---

# Css Animations

Most, if not all modern websites make use of animations. Chances are when you hover your mouse over a link, or tap a button on your
phone / tablet, a css property will change - perhaps a color, or text decoration, or things may even move around.

Today we'll learn how to apply these simple animations to add some sparkle to your sites, and then look at how more complex animations can be made using `keyframes`.

Here is an [example](./index.html) of the power of css animation!

### Animating using Pseudo-classes:

In lesson 17 we took a look at Pseudo-classes. The one we're going to look at for this lesson is `:hover`, though there are plenty more.

let's say we have a menu link with some text:

```css
menu-link {
    color: red;
}
```

```css
menu-link:hover {
    color: blue;
    text-decoration: underline;
}
```

What are we doing here?

-   When a user `hovers` over the menu link element. the color will change, and the text will be underlined.
-   There are lots and lots of css properties we can change like this, but not all.
-   Generally, if a property is part of a range (eg a number, or a color) we can animate like this.

Let's add some hover effects to our websites, or play around with a new html file!

### Actually Animating :D

-   We can change propeties now, but we aren't really animating, we're just changing a property with no smooth transition.
-   This is where our friend transition comes in! transition will make this change across a specified amount of time.

```css
menu-link:hover {
    color: blue;
    text-decoration: underline;
    transition: all 1s ease-in-out 0.5s;
}
```

-   If we were to open our website now, we should see the properties animating over 1 second. But, what is the transition property actually doing?

-   Transition is a `shorthand` (combining multiple css properties in one line, for example margin, border) which covers different properties, below
    is the equivalent of writing as a shorthand:

```css
menu-link:hover {
    color: blue;
    text-decoration: underline;
    transition-property: all;
    transition-duration: 1s;
    transition-timing-function: ease-in-out;
    transition-delay: 0.5s;
}
```

What is each property doing?

-   transition-property: which properties will be animated. we can animate all, or choose 1 or more individually.
-   transition-duration: how long the animation takes
-   transition-timing-function: a little complex, but you can think of it as if the speed of the animation is smooth, or it speeds up, slows down etc.
-   transition-delay: how long after the animtation is trigged, that it should actually begin.

Let's add some transitions!

### Keyframes

coming soon...

## Learn more

-   [Mozilla guide to transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)

```

```
