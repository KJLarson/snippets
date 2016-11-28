---
layout: page
title: Boolean
categories: data types
permalink: /boolean/

---

> A **Boolean** is a value that is either true or false.

```js
var foo = true;
var bar = false;
```

Boolean values are very commonly used in programming for when a value might switch between yes and no, on and off, or true and false. Booleans can represent the current state of something that is likely to change.

For example, we'd use a Boolean to indicate whether a checkbox is checked or not.

```js
var isChecked = true;
```

Often, Booleans are used to check if two things are equal, or if the result of a math equation is true or false.

```js
/* Check if 7 is greater than 8 */
7 > 8; // returns false

/* Check if a variable is equal to a string */
var color = "Blue";

color === "Blue"; // returns true
```

> **Note:** A single equals sign (`=`) applies one value to another. A double (`==`) or triple equals sign (`===`) checks if two things are equal.
