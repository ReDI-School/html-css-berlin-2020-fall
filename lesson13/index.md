---
title: CSS Specificity
nav_order: 13
---

# CSS Specificity

Specificity is a great tool to manage the power of CSS but can be complicated. As we will see, not all selectors are
equal in "power":

- If there are two or more rules that apply to an element, the most specific selector is used
- If the two rules have equal specificity, then the latest rule is applied

Let's check this example. Which one is more important?

```
li {
    color:green;
}
li.special {
    color:red;
}
```

**What about now?**

```
li#special {
    color:green;
}
li.special {
    color:red;
}
```

**How does it works**

- Specificity determines, which CSS rule is applied by the browsers
- Specificity is usually the reason why your CSS-rules don’t apply to some elements, although you think they should
- Every selector has its place in the specificity hierarchy
- If two selectors apply to the same element, the one with higher specificity wins.
- There are four distinct categories which define the specificity level of a given selector: inline styles, IDs,
classes, attributes, and elements
- When selectors have an equal specificity value, the latest rule is the one that counts
- When selectors have an unequal specificity value, the more specific rule is the one that counts
- Rules with more specific selectors have a greater specificity
- The last rule defined overrides any previous, conflicting rules
- The embedded style sheet has a greater specificity than other rules
- ID selectors have a higher specificity than attribute selectors
- You should always try to use IDs to increase the specificity
- A class selector beats any number of element selectors
- The universal selector and inherited selectors have a specificity of 0, 0, 0, 0

**Let's take a look at how the numbers are actually calculated:**

![Specificity](specificity.png)

- If the element has inline styling, that automatically1 wins (1,0,0,0 points)
- For each ID value, apply 0,1,0,0 points
- For each class value (or pseudo-class or attribute selector), apply 0,0,1,0 points
- For each element reference, apply 0,0,0,1 point

You can generally read the values as if they were just a number, like 1,0,0,0 is "1000", and so clearly wins over a
specificity of 0,1,0,0 or "100". The commas are there to remind us that this isn't really a "base 10" system, in that
you could technically have a specificity value of like 0,1,13,4 - and that "13" doesn't spill over like a base 10 system
would.

**Let's see some very good examples**

- [CSS Specificity Wars](https://stuffandnonsense.co.uk/archives/css_specificity_wars.html)
- [CSS Bento Box](https://flukeout.github.io/)


**Learn more**:

- [W3Schools: CSS Specificity](https://www.w3schools.com/css/css_specificity.asp)
- [CSS Tricks: Specifics on CSS Specificity](https://css-tricks.com/specifics-on-css-specificity/)
- [Smashing Magazine: CSS Specificity Things You Should Know](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)

