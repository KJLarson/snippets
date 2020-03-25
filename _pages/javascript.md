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