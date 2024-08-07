---
title: Zebra striped list
type: snippet
language: css
tags: [visual]
cover: forest-balcony
excerpt: Creates a striped list with alternating background colors.
listed: true
dateModified: 2020-12-30
---

Creates a striped list with alternating background colors.

- Use the `:nth-child(odd)` or `:nth-child(even)` pseudo-class selectors to apply a different `background-color` to elements that match based on their position in a group of siblings.

> [!TIP]
>
> You can use it to apply different styles to other HTML elements like `<div>`, `<tr>`, `<p>`, `<ol>`, etc.

```html
<ul>
  <li>Item 01</li>
  <li>Item 02</li>
  <li>Item 03</li>
  <li>Item 04</li>
  <li>Item 05</li>
</ul>
```

```css
li:nth-child(odd) {
  background-color: #999;
}
```
