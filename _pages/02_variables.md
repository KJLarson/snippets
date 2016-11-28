---
layout: page
title: Variables
categories: basics
permalink: /variables/

---

> A **variable** is a container that stores data values.

```js
var foo;
```

You know a variable as something that can change. In basic algebra, it's a letter that represents a number. `x` is a common variable name, but it can just as easily be represented by `y`, `z`, or another name.

Initially `x` has no value or meaning, but you can apply a value to it.

```js
x = 5
```

Now `x` represents `5`. You can think of `x` as a container that's storing `5`, which is a number.

In JavaScript, variables work the same, except they can contain more than just numbers as a value - they can contain all sorts of data values, which we'll learn by the end of this article.

Variables are created and declared using the keyword `var`. We can use our algebra example above to create a JavaScript statement.

```js
var x = 5; // the variable x contains the numeric value of 5.
```

Building on what we've learned so far, you can see that we have a JavaScript statement that declares a variable (`x`), assigns the number data type (`5`) with a single equals sign (`=`), and explains it in plain English with a comment (`//`). The statement ends with a semi-colon (`;`). 

Variables only need to be declared with `var` the first time they're used, and as the name suggests, a variable can change.

```js
var x = 5; // x was worth 5
x = 6; // now it's worth 6
```

A variable can only contain one value at a time, and since the program is executed from top to bottom, the value of `x` is now `6`.

Here is an example of a variable with a different data type.

```js
var greeting = "Oh hi, Mark!";
```

Now the `greeting` variable contains the string `Oh hi, Mark!`.

A few important things to know about variables:

- A variable name can have letters, numbers, a dollar sign (`$`), and an underscore (`_`), but cannot begin with a number.
- A variable cannot be any word on the list of [reserved keywords](http://www.w3schools.com/js/js_reserved.asp).
- Variables are case sensitive.
- The naming convention is **camelCase**, in which a variable always starts lower case, but each subsequent word is uppercase.
- Although a variable can have any name, it's important to choose names that are descriptive yet concise.
