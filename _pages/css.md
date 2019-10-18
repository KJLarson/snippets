---
layout: page
title: CSS
categories: css
subtitle:
permalink: /css/
---

Using flexbox, define the alignment along the main axis:

 ```css
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}
 ```

 Using flexbox, define the alignment along the cross axis:

```css
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}
```