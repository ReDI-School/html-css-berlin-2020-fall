---
title: Fontawesome
nav_order: 20
---

# Fontawesome

Font Awesome is a font and icon toolkit based on CSS. It has a free and a paid version and you can integrate it easily
into your websites to add icons.

## How it works

The free version of Fontawesome has more than 1400 icons that can be accessed with a bit of HTML and a link to an
external css file. You can also download the files and install them on your computer but for websites is easier to do it
online.

First of all, you need to add the css link:

```html
<link rel="stylesheet"
    href="https://use.fontawesome.com/releases/v5.5.0/css/all.css"
    integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU"
    crossorigin="anonymous">
```

<link rel="stylesheet"
    href="https://use.fontawesome.com/releases/v5.5.0/css/all.css"
    integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU"
    crossorigin="anonymous">

Once you do that, you can [search for the icons](https://fontawesome.com/icons?d=gallery&m=free) you want.

## Let's do an example

We will replace the social media networks for their icons.

<p>
    Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">Facebook</a>,
    <a href="https://twitter.com/redischool">Twitter</a>,
    <a href="https://www.instagram.com/redischool/">Instagram</a> and
    <a href="https://www.meetup.com/ReDI-school/">Meetup</a>
</p>

```html
<p>
    Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">Facebook</a>,
    <a href="https://twitter.com/redischool">Twitter</a>,
    <a href="https://www.instagram.com/redischool/">Instagram</a> and
    <a href="https://www.meetup.com/ReDI-school/">Meetup</a>
</p>
```

Now we [open Fontawesome](https://fontawesome.com/v4.7.0/icons/) and search for Facebook icon.

We copy the HTML code `<i class="fab fa-facebook-square" aria-hidden="true"></i>` and replace it for the word "Facebook"
on our code.

```html
<p>Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">
        <i class="fab fa-facebook-square" aria-hidden="true"></i>
    </a>,
    <a href="https://twitter.com/redischool">Twitter</a>,
    <a href="https://www.instagram.com/redischool/">Instagram</a> and
    <a href="https://www.meetup.com/ReDI-school/">Meetup</a>
</p>
```

This is the result

<p>Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">
        <i class="fab fa-facebook-square" aria-hidden="true"></i>
    </a>,
    <a href="https://twitter.com/redischool">Twitter</a>,
    <a href="https://www.instagram.com/redischool/">Instagram</a> and
    <a href="https://www.meetup.com/ReDI-school/">Meetup</a>
</p>

Now we do the same with all the logos

```html
<p>Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">
        <i class="fab fa-facebook-square" aria-hidden="true"></i>
    </a>,
    <a href="https://twitter.com/redischool">
        <i class="fab fa-twitter-square" aria-hidden="true"></i>
    </a>,
    <a href="https://www.instagram.com/redischool/">
        <i class="fab fa-instagram" aria-hidden="true"></i>
    </a> and
    <a href="https://www.meetup.com/ReDI-school/">
        <i class="fab fa-meetup" aria-hidden="true"></i>
    </a>
</p>
```

<p>Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">
        <i class="fab fa-facebook-square" aria-hidden="true"></i>
    </a>,
    <a href="https://twitter.com/redischool">
        <i class="fab fa-twitter-square" aria-hidden="true"></i>
    </a>,
    <a href="https://www.instagram.com/redischool/">
        <i class="fab fa-instagram" aria-hidden="true"></i>
    </a> and
    <a href="https://www.meetup.com/ReDI-school/">
        <i class="fab fa-meetup" aria-hidden="true"></i>
    </a>
</p>

```css
.fab {
    font-size: 1.5rem;
}
.fa-facebook-square {
    color: #3b5998;
}
.fa-twitter-square {
    color: #38A1F3;
}
.fa-instagram {
    color: #fb3958;
}
.fa-meetup {
    color: #e51937;
}
```

<p>Find ReDI School in Social Media:
    <a href="https://www.facebook.com/redischool">
        <i class="fab fa-facebook-square" aria-hidden="true" style="font-size: 1.5rem; color: #3b5998;"></i>
    </a>,
    <a href="https://twitter.com/redischool">
        <i class="fab fa-twitter-square" aria-hidden="true" style="font-size: 1.5rem; color: #38A1F3;"></i>
    </a>,
    <a href="https://www.instagram.com/redischool/">
        <i class="fab fa-instagram" aria-hidden="true" style="font-size: 1.5rem; 1rem; color: #fb3958;"></i>
    </a> and
    <a href="https://www.meetup.com/ReDI-school/">
        <i class="fab fa-meetup" aria-hidden="true" style="font-size: 1.5rem; 1rem; color: #e51937;"></i>
    </a>
</p>

## Learn more

- [Fontawesome](https://fontawesome.com/)
- [W3Schools: Icons Tutorial](https://www.w3schools.com/icons/default.asp)
