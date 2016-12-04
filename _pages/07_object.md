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
var robin  = Object.create(null);
```

Objects are collections of *properties*, which are name-value pairs. This means
that we use a name to access a value. The key can be any valid JavaScript
string, while the value can be any valid JavaScript type or object, including
arrays, maps, and functions. Also, properties that are functions can be called
*methods*.

**Property**       | **Method**
------------       | ----------
`batman.firstName` | `batman.fight()`
`batman.location`  | `batman.jump()`

We can apply some properties to the `batman` object using name-value pairs
(sometimes referred to as *key-value* pairs). They will be comma-separated and
written as `propertyName: propertyValue`.

``` js
var batman = {
   firstName:   "Bruce",   // string
   lastName:    "Wayne",
   location:    "Gotham",
   introduced:  1939,      // number
   billionaire: true,      // boolean
   weakness:    null,      // null
};
```

As you can see, we can apply any primitive data type as a value in an object. We
can retrieve an individual value with a dot (`.`).

``` js
batman.firstName;  // returns "Bruce", a string
```

We can also retrieve the value with bracket notation.

``` js
batman["firstName"];  // returns "Bruce"
```

A JavaScript property name must be a valid JavaScript string or numeric literal.
If the name begins with a number, has a space or hypen, then it must be accessed
using the bracket notation. [Read: MDN][1]

``` js
batman.secret identity;     // invalid
batman["Secret Identity"];  // valid
```

A method performs an action. Here is a simple example.

``` js
var batman = {
   firstName: "Bruce",
   lastName: "Wayne",

   // properties which are functions are called 'methods'
   secretIdentity: function() {
      return this.firstName + " " + this.lastName;
   },
};
```

While the properties `firstName` and `lastName` are strings, `secretIdentity` is
a function. Instead of manually combining the values of `firstName` and
`lastName` myself, we can use the `secretIdentity` method.

Instead of a simple data type as the value, I have a `function`. The `function`
is concatenating `firstName` and `lastName` for `this` object and returning the
result. In the example, `this` is the same as `batman` because it's inside the
object (`{}`).

``` js
batman.secretIdentity(); // returns "Bruce Wayne", a concatenation of two properties
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
  "Donatello",
];
```

You can get an individual value by referencing the `index` of the array. In
programming, counting starts at zero, so the first item in a list will always
be `[0]`.

``` js
var leader = ninjaTurtles[0]; // assigns "Leonardo" to the leader variable
```

You can see how many items are in an array with `length`.

``` js
ninjaTurtles.length; // returns 4
```

[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Objects_and_properties
