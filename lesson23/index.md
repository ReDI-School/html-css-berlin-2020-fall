---
title: CSS Animations Part 2
nav_order: 23
---

# CSS Animations Part 2

Let's take a look at some more CSS animation concepts:

-   Transforms
-   Keyframes

## The CSS Property Transform:

This handy property lets us move an element, rotate it, distort it, or change the size.

Tranform types:

-   rotate
-   scale (increase / decrease size)
-   skew (distort)
-   translate (aka move across 2d / 3d planes)

We can combine these types, and do some really powerful things with it, but it means that using the property can get quite complex. Let's stick to some simple examples for now, as we learn and practice!

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

You might be wondering if I can just do something like this:

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

The answer is a little complex, and beyond the scope of our course; but basically, it's easier for the browser to change size or position using transform, than changing the height/width, etc directly. This means your animations will be much smoother!

## The CSS Property Keyframes:

Keyframes allow us to make complex multistep animations, compared to transitions.

Here is a very simple example:

```css
@keyframes slidein {
  from {
    transform: translateX(0%);
  }

  to {
    transform: translateX(100%);
  }
}
```

- We define the start point (from), as a `transform` of `translateX(0)`, and the end point as a `transform` of `translateX(0)`. 

- We can use percentages as well:

```css
@keyframes slideinOut {
  0% { transform: translateX(0%); }
  25% { transform: translateX(25%); }
  50% { transform: translateX(50%); }
  75% { transform: translateX(25%); }
  100% { transform: translateX(0%); }
}
```

### how do we use these animations?

We can 'apply' the animatiion to a selector, for example:

```css
.promoBanner {
    animation-duration: 3s;
    animation-name: slideinOut;
}
```

Similar to how we use transition, we add the `animation-name` property, to the element/s we want to animate.

Other useful properties:

- `animation-iteration-count: infinite;` will repeat the animation constantly.
- `animation-direction: alternate;` will run the animation first forward, then in reverse.
- `animation-delay: 2s` delays the start of the animation, same as transition delay
- `animation-timing-function: linear` works the same as our tranisition timing function, controls the 'velocity' of the animation.

We can use a shorthand for our animation properties. The below examples, do the same thing.

```css 
{
  animation-name: test;
  animation-duration: 1s;
  animation-timing-function: ease-in;
  animation-delay: 0.5s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}

{
  animation: test 1s ease-in 0.5s infinite alternate;
}
```

## Learn more

-   [W3 Schools: CSS @keyframes Rule](https://www.w3schools.com/cssref/css3_pr_animation-keyframes.asp)
-   [W3 Schools: Css Animations](https://www.w3schools.com/css/css3_animations.asp)
-   [Mozilla: Using Css animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations)
