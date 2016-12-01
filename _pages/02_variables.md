---
layout: page
title: Variables
subtitle: A container that stores data values.
categories: basics
permalink: /variables/

---

You know a variable as something that can change. In basic algebra, it's a letter that represents a number. `x` is a common variable name, but it can just as easily be represented by `y`, `z`, or another name. In JavaScript, variables work the same, except they can contain more than just numbers as a value - they can contain all sorts of data values.

```js
var x = 5; // the variable x contains the numeric value of 5.
```

In this case, `x` represents `5`. You can think of `x` as a container that's storing `5`, which is a number. Variables are created and declared using the keyword `var`. Variables only need to be declared with `var` the first time they're used, and as the name suggests, a variable can change.

```js
var x = 5; // x was worth 5
x = 6; // now it's worth 6
```

### Rules

- A variable name can have letters, numbers, a dollar sign (`$`), and an underscore (`_`), but cannot begin with a number.
- A variable cannot be any word on the list of [reserved keywords](http://www.w3schools.com/js/js_reserved.asp).
- Variables are case sensitive.
- The naming convention is **camelCase**, in which a variable always starts lower case, but each subsequent word is uppercase.
