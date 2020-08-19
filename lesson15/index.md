---
title: HTML Tables
nav_order: 15
---

# HTML Tables

The table element represents data with more than one dimension, in the form of a table. Tables have rows, columns, and cells given by their descendants. The rows and columns form a grid; a table’s cells must completely cover that grid without overlap.

An HTML table is defined with the `<table>` tag.

Each **table row** is defined with the <tr> tag. A **table header** is defined with the `<th>` tag. By default, table headings are bold and centered. A **table data/cell** is defined with the `<td>` tag.

Example 

<table style="width: 50%;" border="1">
    <caption>
      Bundesliga
    </caption>
    <tr>
      <th>Position</th>
      <th>Team</th>
      <th>Matches Played</th>
      <th>Points</th>
    </tr>
    <tr>
      <td>1</td>
      <td>Dortmund</td>
      <td>6</td>
      <td>16</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Hoffenheim</td>
      <td>6</td>
      <td>14</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Bayern Muenchen</td>
      <td>6</td>
      <td>13</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Hannover 96</td>
      <td>6</td>
      <td>12</td>
    </tr>
  </table>




```
 <table>
    <caption>
      Bundesliga
    </caption>
    <tr>
      <th>Position</th>
      <th>Team</th>
      <th>Matches Played</th>
      <th>Points</th>
    </tr>
    <tr>
      <td>1</td>
      <td>Dortmund</td>
      <td>6</td>
      <td>16</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Hoffenheim</td>
      <td>6</td>
      <td>14</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Bayern Muenchen</td>
      <td>6</td>
      <td>13</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Hannover 96</td>
      <td>6</td>
      <td>12</td>
    </tr>
  </table>
  ```


The `<thead>` tag is used to group header content in an HTML table. It is used in conjunction with the `<tbody>` and `<tfoot>` elements to specify each part of a table (header, body, footer).

Browsers can use these elements to enable scrolling of the table body independently of the header and footer. Also, when printing a large table that spans multiple pages, these elements can enable the table header and footer to be printed at the top and bottom of each page.

### Examples

Another examples of tables can be found in tennis scoreboards, stock markets, weather widgets, calendars etc. Tables offer interesting styling options. We can practice with this [stock market table](./nasdaq.html).

## Learn more

- [W3Schools: HTML Tables](https://www.w3schools.com/html/html_tables.asp)
- [CSS-Tricks: A Complete Guide to the Table Element](https://css-tricks.com/complete-guide-table-element/)