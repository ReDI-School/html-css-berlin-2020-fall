---
title: Responsive Web Design — CSS Media Queries
nav_order: 19
---

# CSS Media Queries

The **@media** rule made it possible to define different style rules for different media types. That way you could have 
one set of style rules for computer screens, one for printers, one for handheld devices, one for television-type 
devices, and so on.

Unfortunately these media types never got a lot of support by devices, other than the print media type.

A newer version of Media queries extended the media types idea: Instead of looking for a type of device, they look at 
the capability of the device.

Media queries can be used to check many things, such as:

- width and height of the viewport
- width and height of the device
- orientation (is the tablet/phone in landscape or portrait mode?)
- resolution

Using media queries are a popular technique for delivering a tailored style sheet to desktops, laptops, tablets, and 
mobile phones (such as iPhone and Android phones).

## How to write media queries

```css
@media screen and (max-width: 480px) {
    body {
        font-size: 125%;
    }
}
```

This declaration says that the text should increase by 25% when the screen is 480px wide or smaller. The value "480px" 
is called a breakpoint.

You can also use ranges for the media queries. In the following example, the change will happen if the screen size is 
between 480 and 800px. The breakpoints are two now: 480px and 800px.

```css
@media screen and (min-width: 480px) and (max-width: 800px) {
    body {
        font-size: 125%;
    }
}
```

## Learn more

- [W3 Schools: CSS Media Queries - Examples](https://www.w3schools.com/css/css3_mediaqueries_ex.asp)
