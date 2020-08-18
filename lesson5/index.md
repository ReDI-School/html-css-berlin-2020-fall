---
title: HTML Basics
nav_order: 5
---

# HTML Basics

**Doctype, headings, paragraphs, lists**

## The <!DOCTYPE> Declaration

The <!DOCTYPE> Declaration represents the document type, and helps browsers to display web pages correctly. It must only
appear once, at the top of the page (before any HTML tags).

- The `<!DOCTYPE>` declaration is not case sensitive.
- The `<!DOCTYPE>` declaration for HTML5 is: `<!DOCTYPE html>`

## HTML basics

- All HTML documents must start with a document type declaration: `<!DOCTYPE html>`.
- The HTML document itself begins with `<html>` and ends with `</html>`.
- The visible part of the HTML document is between `<body>` and `</body>`.
- HTML headings are defined with the `<h1>` to `<h6>` tags.
- `<h1>` defines the most important heading.
- `<h6>` defines the least important heading.
- HTML paragraphs are defined with the `<p>` tag: `<p>This is a paragraph</p>`.

## Examples

<h1>This is h1, the biggest HTML heading</h1>
<h2>This is h2, smaller than h1</h2>
<h3>This is h3, as you've guessed</h3>
<h4>This is how the h4 looks like</h4>
<h5>This is h5, quite small</h5>
<h6>This is h6, the smallest one</h6>
<p>This is a paragraph. Browsers do not display the HTML tags, but use them to render the content of the page. It's
important to use the right HTML tags for each content element. Semantics are important: a well structured HTML document
will be rendered correctly by all browsers and properly scanned and stored by the search engines.</p>

## Quick Exercise

Take the HTML file that you code before (the one with `h1` and `p`) and add `h2`, `h3`, `h4`, `h5` and `h6`.

**IMPORTANT**: Remember to always close the tags; if you open with `<h3>`, you close with `</h3>`.

## Unordered and ordered lists

Lists are one of the most used HTML tags. There are two kind of lists:

## Unordered Lists

<ul>
  <li>This is the first item</li>
  <li>This is the second item</li>
  <li>This is the third item</li>
  <li>This is the fourth item</li>
</ul>

## Ordered Lists

<ol>
  <li>This is the first item</li>
  <li>This is the second item</li>
  <li>This is the third item</li>
  <li>This is the fourth item</li>
</ol>

## Another Quick Exercise

Now add two lists to the HTML file: `ol` and `ul`.

**IMPORTANT**: Remember that each item on a list should open with `<li>` and closed with `</li>`.

## Exercise on paper

Let's recognize headings, paragraphs and lists on our paper websites

1. Using a colored marker, write on your website which elements you are using:
2. Mark the different headings as `h1`, `h2`, `h3`...
3. Mark all the paragraphs
4. Do you have lists?
5. Mark the navigation as a list

**Learn more**:

- [W3Schools: HTML Documents, Headings, Paragraphs and Lists](https://www.w3schools.com/html/html_basic.asp)
