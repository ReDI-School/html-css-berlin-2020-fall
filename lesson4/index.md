---
title: What is HTML?
nav_order: 4
---

# What is HTML?

Hypertext Markup Language (HTML) is the standard markup language for creating web pages and web applications. With
Cascading Style Sheets (CSS) and JavaScript, it forms a triad of cornerstone technologies for the World Wide Web.

- Hypertext Markup Language: HTML is a language for writing documents
- Hypertext: Documents link to each other
- Markup: Describes the semantic role of parts of a document

## Semantic Markup

Many HTML tags have semantic meaning. That is, the element itself conveys some information about the type of content
contained between the opening and closing tags. With semantic markup the tags themselves become a way to tell a machine
(whether a browser, a computer, a smartphone, or another smart device) something about the meaning of the content.

## HTML structure

**Heading**: it contains informations about the document such as title, scripts, styles, meta information, and more:

```
    <head></head>
```

**Body**: it contains everything you see on the web: text, images, graphic and other elements.

```
    <body></body>
```

## HTML Tags

HTML tags are element names surrounded by angle brackets: `<tagname>content goes here...</tagname>`

- HTML tags normally come in pairs like `<p> and </p>`

- The first tag in a pair is the start tag, the second tag is the end tag
- The end tag is written like the start tag, but with a forward slash inserted before the tag name
- **Tip**: The start tag is also called the opening tag, and the end tag the closing tag.

## HTML Page Structure

Below is a visualization of an HTML page structure:

```
<!DOCTYPE html>
<html>

    <head>
        <title>Page title</title>
    </head>

    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
        <p>This is another paragraph.</p>
    </body>

</html>
```

**Note**: Only the content inside the `<body>` section is displayed in a browser.

## Exercise: let's code our first HTML document

Let's all follow these steps:

1. On the desktop of your computer, create a folder called ReDI HTML&CSS Lessons
2. Inside that folder, create another folder called First Exercise
3. Open Atom
4. Create a new file (File > New File or with Control + N)
5. Save the file as index.html inside the First Exercise folder
6. Write the code that we show above this list.
7. Open the file with **Chrome** to see how it looks.
8. Yes, it looks great.

**Learn more**:

- [W3Schools: HTML Introduction](https://www.w3schools.com/html/html_intro.asp)
- [W3Schools: HTML Editors](https://www.w3schools.com/html/html_editors.asp)
- [W3Schools: HTML Semantic](https://www.w3schools.com/html/html5_semantic_elements.asp)
