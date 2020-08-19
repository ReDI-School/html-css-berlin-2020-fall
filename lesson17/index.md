---
title: Pseudo-classes and pseudo-elements
nav_order: 17
---

# Pseudo-classes and pseudo-elements

## What are Pseudo-classes?

A pseudo-class is used to define a special state of an element. For example, it can be used to:

- Style an element when a user mouses over it
- Style visited and unvisited links differently
- Style an element when it gets focus

### Syntax

```
selector:pseudo-class {
  property: value;
}
```

### A common example: anchor Pseudo-classes

- Unvisited: a:link
- Visited: a:visited
- Mouse Over: a:hover
- Selected: a:active

### All CSS Pseudo Classes

| Selector | Example | Description |
| --- | --- | --- |
| [:active](https://www.w3schools.com/cssref/sel_active.asp) | a:active | Selects the active link |
| [:checked](https://www.w3schools.com/cssref/sel_checked.asp) | input:checked | Selects every checked `<input>` element |
| [:disabled](https://www.w3schools.com/cssref/sel_disabled.asp) | input:disabled | Selects every disabled `<input>` element |
| [:empty](https://www.w3schools.com/cssref/sel_empty.asp) | p:empty | Selects every `<p>` element that has no children |
| [:enabled](https://www.w3schools.com/cssref/sel_enabled.asp) | input:enabled | Selects every enabled `<input>` element |
| [:first-child](https://www.w3schools.com/cssref/sel_firstchild.asp) | p:first-child | Selects every `<p>` elements that is the first child of its parent |
| [:first-of-type](https://www.w3schools.com/cssref/sel_first-of-type.asp) | p:first-of-type | Selects every `<p>` element that is the first `<p>` element of its parent |
| [:focus](https://www.w3schools.com/cssref/sel_focus.asp) | input:focus | Selects the `<input>` element that has focus |
| [:hover](https://www.w3schools.com/cssref/sel_hover.asp) | a:hover | Selects links on mouse over |
| [:in-range](https://www.w3schools.com/cssref/sel_in-range.asp) | input:in-range | Selects `<input>` elements with a value within a specified range |
| [:invalid](https://www.w3schools.com/cssref/sel_invalid.asp) | input:invalid | Selects all `<input>` elements with an invalid value |
| [:lang(language)](https://www.w3schools.com/cssref/sel_lang.asp)| p:lang(it)| Selects every `<p>` element with a lang attribute value starting with "it" |
| [:last-child](https://www.w3schools.com/cssref/sel_last-child.asp) | p:last-child | Selects every `<p>` elements that is the last child of its parent |
| [:last-of-type](https://www.w3schools.com/cssref/sel_last-of-type.asp) | p:last-of-type | Selects every `<p>` element that is the last `<p>` element of its parent  |
| [:link](https://www.w3schools.com/cssref/sel_link.asp)| a:link | Selects all unvisited links  |
| [:not(selector)](https://www.w3schools.com/cssref/sel_not.asp) | :not(p) | Selects every element that is not a `<p>` element |
| [:nth-child(n)](https://www.w3schools.com/cssref/sel_nth-child.asp) | p:nth-child(2) | Selects every `<p>` element that is the second child of its parent  |
| [:nth-last-child(n)](https://www.w3schools.com/cssref/sel_nth-last-child.asp) | p:nth-last-child(2) | Selects every `<p>` element that is the second child of its parent, counting from the last child |
| [:nth-last-of-type(n)](https://www.w3schools.com/cssref/sel_nth-last-of-type.asp) | p:nth-last-of-type(2) | Selects every `<p>` element that is the second `<p>` element of its parent, counting from the last child |
| [:nth-of-type(n)](https://www.w3schools.com/cssref/sel_nth-of-type.asp)| p:nth-of-type(2) | Selects every `<p>` element that is the second `<p>` element of its parent |
| [:only-of-type](https://www.w3schools.com/cssref/sel_only-of-type.asp) | p:only-of-type | Selects every `<p>` element that is the only `<p>` element of its parent |
| [:only-child](https://www.w3schools.com/cssref/sel_only-child.asp) | p:only-child | Selects every `<p>` element that is the only child of its parent  |
| [:optional](https://www.w3schools.com/cssref/sel_optional.asp) | input:optional | Selects `<input>` elements with no "required" attribute |
| [:out-of-range](https://www.w3schools.com/cssref/sel_out-of-range.asp) | input:out-of-range | Selects `<input>` elements with a value outside a specified range |
| [:read-only](https://www.w3schools.com/cssref/sel_read-only.asp) | input:read-only  | Selects `<input>` elements with a "readonly" attribute specified |
| [:read-write](https://www.w3schools.com/cssref/sel_read-write.asp) | input:read-write | Selects `<input>` elements with no "readonly" attribute |
| [:required](https://www.w3schools.com/cssref/sel_required.asp) | input:required | Selects `<input>` elements with a "required" attribute specified  |
| [:root](https://www.w3schools.com/cssref/sel_root.asp)| root | Selects the document's root element |
| [:target](https://www.w3schools.com/cssref/sel_target.asp) | #news:target | Selects the current active #news element (clicked on a URL containing that anchor name) |
| [:valid](https://www.w3schools.com/cssref/sel_valid.asp) | input:valid| Selects all `<input>` elements with a valid value |
| [:visited](https://www.w3schools.com/cssref/sel_visited.asp) | a:visited | Selects all visited links |



## What are Pseudo-Elements?

A CSS pseudo-element is used to style specified parts of an element. For example, it can be used to:

- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

Notice the double colon notation - **::first-line** versus **:first-line**

The double colon replaced the single-colon notation for pseudo-elements in CSS3. This was an attempt from W3C to distinguish between pseudo-classes and pseudo-elements. The single-colon syntax was used for both pseudo-classes and pseudo-elements in CSS2 and CSS1.

### CSS - The ::after Pseudo-element

The **::after** pseudo-element can be used to insert some content after the content of an element. The **::before** pseudo-element insert the content before the element. Obviously.

## Learn more

- [W3Schools: Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp)
- [W3Schools: Pseudo-elements ](https://www.w3schools.com/css/css_pseudo_elements.asp)
- [CSS-Tricks: A Whole Bunch of Amazing Stuff Pseudo Elements Can Do](https://css-tricks.com/pseudo-element-roundup/)
- [CSS-Tricks: Glyphs](https://css-tricks.com/snippets/html/glyphs/)