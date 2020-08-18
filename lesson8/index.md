---
title: HTML Basics - More Exercises
nav_order: 8
---

# HTML Basics - More Exercises

## What we have learned so far

In these first weeks we've learned the basic HTML tags and did a couple of exercises. Let's review them again before
going back to our websites. This is what we've learned:

- **Headings**: use `h1` to `h6`
- **Paragraphs**: use `p`
- **Unordered lists**: write them with `ul`. Each item on the list is wrapped with `li`
- **Ordered lists**: write them with `ol`. Each item on the list is wrapped with `li`
- **Links**: you open the link with `a href=""` and close it with `/a`. Inside the quotes you write where the link will
point to
- **Image links**: Instead of wrapping text with `<a href="">` and `</a>`, you wrap an image.
- **HTML comments**: Anything you place between `<!--` and `-->` will be hidden for the browsers.

## Exercises

### Which code snippet is right?

Please compare carefully [the four options](./correct-render.pdf) and choose the correct one.

### Find the errors

You can see the examples below or [check the errors on a pdf](./find-the-errors.pdf).

```
EXAMPLE ONE

<h1>Welcome to ReDI school!</h2>
<p>We are learning how to do a page with</p>
<ul>
    <li>headings</li>
    <li>paragraphs</li><!--
    <li>unordered lists</li>
    <li>ordered lists
    </li>
    <li>images</li>
    <li>links</li>
    <li>comments</li>
</ul>


EXAMPLE TWO

<h2>Welcome to ReDI school!</h2>
<p>We are learning how to do a page with</p>
<h3>
    <li>headings</li>
    <li>paragraphs</li>
    <li>unordered lists</li>
    <li>ordered lists</li>
    <li>images</li>
    <ul>links</li>
    <li>comments</ul>
</h3>


EXAMPLE THREE

<h1>Welcome to ReDI school!</h1>
<ul>
<p>We are learning how to do a page with</p>
    <li>headings</li>
    <li>paragraphs</li>
    <li>unordered lists</li>
    <li>ordered lists</li>
    <li>images</li>
    <li>links</li>
    <li>comments</li>
</ul>
```

### This is the HTML; what will the browser show?

```
<!-- Welcome -->
<h1>Welcome to ReDI school!</h1>
<p>We are learning how to do a page with</p>
<ul>
    <li>headings</li><!-- h1 to h6 -->
    <li>paragraphs</li><!--
    --><li>unordered lists</li>
    <li>ordered lists</li>
    <li>images</li>
    <li>links</li><!--
    <li>comments</li>-->
</ul>
```

