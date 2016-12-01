---
layout: page
title: Number
subtitle:  A numerical value.
categories: data types
permalink: /number/

---

Numbers do not have any special syntax associated with them like strings do. If you were to place a number in quotes (`"5"`), it wouldn't be considered a number, but a character in a string. A number can be whole or a decimal (known as a float), and can have a positive or negative value. A number can have up to 15 digits.

```js
var x = 5; // whole integer
var y = 1.2; // float
var z = -76; // negative whole integer
var largeNumber = 999999999999999; // a valid number
```

You can do regular math with numbers - addition (`+`), subtraction (`-`), division (`/`), multiplication (`+`) and modulus (`%`).

```js
var sum = 2 + 5; // returns 7
var difference = 6 - 4; // returns 2
```

### NaN

`NaN` means **Not a Number**, even though it's technically a number type. `NaN` is the result of attempting to do impossible math with other data types. Attempting to divide a number by a string, for example, results in `NaN`.

```js
var nope = 1 / "One"; // returns NaN
```

### Infinity

`Infinity` is also technically a number, either the product of dividing by `0` or calculating a number too large.

```js
var beyond = 1 / 0; // returns Infinity
```
