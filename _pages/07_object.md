---
layout: page
title: Object
subtitle: A collection of name/value pairs.
categories: data types
permalink: /object/
---

Any value that isn't simply a string, number, Boolean, null, undefined, or
Symbol is an object.

Create an object with a pair of curly braces (`{}`).

``` js
var batman = {};
```

Objects consist of **properties** and **methods**. Properties are what the
object *is*, and methods are what the object *does*. Returning to the book
analogy, properties are like nouns and adjectives, and methods are like verbs.

**Property**       | **Method**
------------       | ----------
`batman.firstName` | `batman.fight()`
`batman.location`  | `batman.jump()`

We can apply some properties to the `batman` object using name/value pairs
(sometimes referred to as *key/value* pairs). They will be comma-separated and
written as `propertyName: propertyValue`.

``` js
var batman = {
  firstName: "Bruce",  // string
  lastName: "Wayne",
  location: "Gotham",
  introduced: 1939,    // number
  billionaire: true,   // boolean
  weakness: null,      // null
};
```

As you can see, we can apply any primitive data type as a value in an object. We
can retrieve an individual value with a dot (`.`).

``` js
batman.firstName; // returns Bruce, a string
```

We can also retrieve the value with bracket notation.

``` js
batman["firstName"]; // returns Bruce
```

A JavaScript property name must be a valid JavaScript string or numeric literal.
If the name begins with a number or has a space, it must be accessed using the
bracket notation. [Read: MDN][1]

``` js
batman.secret identity; // invalid
batman["Secret Identity"]; // valid
```

A method performs an action. Here is a simple example.

``` js
var batman = {
  firstName: "Bruce",
  lastName: "Wayne",
  secretIdentity: function() { // method
    return this.firstName + " " + this.lastName;
  }
};
```

Instead of a simple data type as the value, I have a `function`. The `function`
is concatenating `firstName` and `lastName` for `this` object and returning the
result. In the example, `this` is the same as `batman` because it's inside the
object (`{}`).

``` js
batman.secretIdentity(); // returns Bruce Wayne, a concatenation of two properties
```

A method is indicated by parentheses. (`()`).

> **Note:** - the last item in a list of objects does not end in a comma.

### Arrays

An **array** stores a list into a single variable.

Since an array contains more than one value, it's a type of object. Create an
array with a pair of straight braces (`[]`).

``` js
var ninjaTurtles = [];
```

Arrays do not contain name/value pairs.

``` js
var ninjaTurtles = [
  "Leonardo",
  "Michelangelo",
  "Raphael",
  "Donatello"
];
```

You can get an individual value by referencing the `index` of the array. In
programming, counting starts at zero, so the first item in a list will always
be `[0]`.

``` js
var leader = ninjaTurtles[0]; // applies Leonardo to the leader variable
```

You can see how many items are in an array with `length`.

``` js
ninjaTurtles.length; // returns 4
```

[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Objects_and_properties
