---
layout: page
title: String
subtitle: A series of characters.
categories: data types
permalink: /string/

---

Any data that contains text will be represented in a string. The name *string* likely originated from early programmers who were reminded of beads on a string.

- A string can be wrapped in **double quotes** (`" "`)  or **single quotes** (`' '`):

```js
"A string with double quotes."; // double quoted string
'A string with single quotes.'; // single quoted string
```

> **Note:** Single quotes are what you would usually call an apostrophe, not to be confused with a backtick, which is located all the way on the left of the keyboard.

Both ends of the string must match, but otherwise there is no difference between the two; they're just different ways of writing a string. It's important throughout a project to choose one style of strings for consistency. However, there are times that you might want to use an apostrophe in a single-quoted string, or quotation marks in a double-quoted string. There are two ways to accomplish this:

Use the opposite type of quote to avoid breaking the string:

```js
"I'm using single quotes in a double quoted string."; // using single quotes in a double quoted string
'Using "double quotes" in a single quoted string.'; // using double quotes in a single quoted string
```

Use a backslash (`\`) to *escape* the string:

```js
'I\'m using single quotes in a double quoted string.'; 
"Using \"double quotes\" in a single quoted string.";
```
