---
layout: page
title: String
subtitle: A string is a series of characters.
categories: data types
permalink: /string/

---

```js
var foo = "Bar";
```

Any data that contains text will be represented in a string. The name *string* likely originated from early programmers who were reminded of beads on a string.

- A string can be wrapped in **double quotes** (`" "`):

```js
"Pull the string, and it will follow wherever you wish."; // double quoted string
```

- or **single quotes** (`' '`):

```js
'Push it, and it will go nowhere at all.'; // single quoted string
```

> **Note:** Single quotes are what you would usually call an apostrophe, not to be confused with a backtick, which is located all the way on the left of the keyboard.

Both ends of the string must match, but otherwise there is no difference between the two - they're just different ways of writing a string.

But what if I want to write *I'm* in a single quoted string, or quote someone in a double quoted string? Won't that break the string?

It will, and there are two options to combat that. You can safely use the opposite type of quotes:

```js
"Damn it, man, I'm a doctor, not a torpedo technician!"; // using single quotes in a double quoted string
'"Do. Or do not. There is no try." - Yoda'; // using double quotes in a single quoted string
```

It's important throughout a project to choose one style for strings for consistency. You can use a backslash (`\`) to *escape* the string.

```js
'Damn it, man, I\'m a doctor, not a torpedo technician!'; 
"\"Do. Or do not. There is no try.\" - Yoda";
```

We can apply strings to variables. Let's use my `greeting` example.

```js
var greeting = "Oh hi, Mark!";
```

Strings can also be linked together in a process known as **concatenation**. Variables and strings can be joined together using the plus (`+`) symbol.

```js
var greeting = "Oh hi, " + "Mark" + "!"; // returns Oh hi, Mark!
```

Note that an empty space is also a character in a string. In the below example, we'll see how concatenation can be useful.

```js
var message = "Oh hi, ";
var firstName = "Mark";
var bam = "!";

var greeting = message + firstName + bam; // returns Oh hi, Mark!
```

Now all the strings are represented by variables which can change. If you've ever logged into email or an app and were greeted with your name, you can see how your name is just a string in a variable in their system.
