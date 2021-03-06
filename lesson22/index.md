---
title: CSS Animations Part 1
nav_order: 22
---

# CSS Animations Part 1

Most, if not all modern websites make use of animations. Chances are when you hover your mouse over a link or tap a button on your phone/tablet, a CSS property will change - perhaps a color, or text-decoration, or things may even move around.

In this lesson, we'll learn how to apply these simple animations to add some sparkle to your sites!

Here is an [example](./sunset.html) of the power of CSS animation!

### Animating using Pseudo-classes:

In lesson 17 we took a look at Pseudo-classes. The one we're going to look at for this lesson is `:hover`, though there are plenty more.

let's say we have a menu link with some text:

```css
.menu-link {
    color: red;
}
```

```css
.menu-link:hover {
    color: blue;
    text-decoration: underline;
}
```

What are we doing here?

-   When a user `hover`s over the menu link element, the color will change, and the text will be underlined.
-   There are lots and lots of CSS properties we can animate, but not all.
-   Generally, if a property is part of a range (eg a number, or a color) we can animate like this.

Let's add some hover effects to our websites, or play around with a new HTML file!

### Actually Animating :D

-   We can change properties now, but we aren't really animating, we're just changing going from one state to another instantly.
-   This is where our friend `transition` comes in!

```css
.menu-link:hover {
    color: blue;
    text-decoration: underline;
    transition: all 1s ease-in-out 0.5s;
}
```

-   If we were to open our website now, we should see the properties animating when we trigger them. But, what is the transition property actually doing?
-   Transition is a `shorthand` (combining multiple CSS properties in one line, for example, margin, border) which covers different properties, below
    is the equivalent of writing as a shorthand:

```css
.menu-link:hover {
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
-   transition-duration: how long the animation takes.
-   transition-timing-function: a little complex, but you can think of it as if the speed of the animation is smooth, or it speeds up, slows down, etc.
-   transition-delay: how long after the animation is triggered, that it should actually begin.

Let's add some transitions!

## Learn more

-   [Mozilla: Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)
