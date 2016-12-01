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

Both ends of the string must match, but otherwise there is no difference between the two - they're just different ways of writing a string. But what if I want to write *I'm* in a single quoted string, or quote someone in a double quoted string? Won't that break the string? It will, and there are two options to combat that. You can safely use the opposite type of quotes:

```js
"I'm using single quotes in a double quoted string."; // using single quotes in a double quoted string
'Using "double quotes" in a single quoted string.'; // using double quotes in a single quoted string
```

It's important throughout a project to choose one style for strings for consistency. You can use a backslash (`\`) to *escape* the string.

```js
'I\'m using single quotes in a double quoted string.'; 
"Using \"double quotes\" in a single quoted string.";
```
