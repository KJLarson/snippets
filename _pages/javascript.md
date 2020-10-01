---
layout: page
title: JavaScript
subtitle: 
categories: javascript
permalink: /javascript/
---

Switch - Execute code based on whether an expression matches a value:

```js
switch (expression) {
  case x:
    // do something
    break;
  case y:
    // do something else
    break;
  case z:
    // do something else
    break;
  default:
    // default code block
    break;
}
```

Ternary operator:
- the condition comes before the <code>?</code>
- two expressions come after the <code>?</code> and are separated by a colon <code>:</code>
- if <code>true</code>, then first expression executes
- if <code>false</code>, the second expression executes

```js
(condition) ? console.log('The condition is true') : console.log('The condition is false');
```

Function expressions (anonymous functions):

```js
  const functionName = function(paramOne, paramTwo) {
    // do something
  }
```

Arrow functions:

Zero parameters
```js
const functionName = () => {};
```

One parameter
```js
const functionName = paramOne => {};
```

Two or more parameters
```js
const functionName = (paramOne, paramTwo) => {};
```

Single-line block (does not need curly braces nor the <code>return</code> keyword)
```js
const sumNumbers = number => number + number;
```

Multi-line block (needs <code>return</code> keyword)
```js
const sumNumbers = number => {
  const sum = number + number;
  return sum;
};
```

Function to create new HTML element:
```js
const createNode = (elem) => {
  return document.createElement(elem);
};
```

Function to append HTML element to parent element:
```js
const appendNode = (parent, elem) => {
  parent.appendChild(elem);
};
```