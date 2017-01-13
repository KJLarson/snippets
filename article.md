So you've decided to learn JavaScript, the programming language of the web. If it seems like a daunting journey ahead and you don't know where to start, here's a little secret: it doesn't take any special skill to learn how to program, and everyone starts at zero. Take it one step at a time, and you'll get there.

## Is This Guide For Me?

If any of these apply to you, you'll benefit from reading this guide:

- You've never used a programming language before.
- You've never used JavaScript before.
- You've tried learning JavaScript before, but found the resources lacking or hard to follow.
- You know a bit of JavaScript, but want to touch up on the basics.

In this article, we're going to focus on the fundamentals: syntax, variables, comments, and data types. The beauty is that you can apply the concepts you learn about JavaScript here to learning another programming language in the future.

> **Disclaimer:** This guide is meant for complete beginners to JavaScript and programming. As such, many concepts will be presented in a simplified manner, and strict ES5 syntax will be used.

Ready? Let's get started!

## What is JavaScript?

JavaScript is the programming language used to make websites dynamic and interactive. It's a **client-side** programming language, which means the code gets executed in the user's web browser. With the advent of [Node.js](https://nodejs.org/en/) and other technologies, it can also be used as a **server-side** language, making it extremely versatile. JavaScript is used primarily for **front-end web development**, and works closely with HTML and CSS.

> **Note:** Java is not JavaScript. It's a different language with a confusingly similar name.

### Requirements

You already have the prerequisites to start writing and using JavaScript. All you need is a **web browser** to view the code, and a **text editor** to write it. The browser you're currently using is perfect (Chrome, Firefox, Safari, Edge, etc). Your computer comes preinstalled with Notepad (Windows) or TextEdit (Mac), but I would recommend installing [Atom](https://atom.io/) or [Brackets](http://brackets.io/), which are free programs specifically designed for coding.

[CodePen](http://codepen.io/) is a website that allows you to write code and make live demos, and it will be the easiest way to start following along and practicing.

### Basic Terminology

A programmer writes programs, just as an author writes a book. 

A **program** is just a set of instructions that a computer can read and use to perform a task. Each individual instruction is a line of code known as a **statement**, which is similar to a sentence in a book. While a sentence in English ends with a period, a JavaScript statement usually ends in a semi-colon. **Syntax** refers to the symbols and rules that define the structure of the language, similar to grammar and punctuation, and the semi-colon that ends a JavaScript statement is part of the syntax.

## Comments

A **comment** is a human-readable note written in the code.

Comments are written in plain English with the purpose of explaining code. Although comments don't technically perform any function in the program, it's crucial to get into the habit of proper documentation to help you or future collaborators understand the intent of your code.

There are two types of comments in JavaScript:

- **A single line comment**, written as two forward slashes `//` followed by the comment.

```js
// This is a single line comment.
```

- **A multi line comment**, which is sandwiched between `/*` and `*/` and can span many lines.

```js
/* This is a comment.
It's a multi line comment.
Also a haiku. */
```

## Variables

A **variable** is a container that stores data values.

You know a [variable](https://www.sitepoint.com/how-to-declare-variables-javascript/) as something that can change. In basic algebra, it's a letter that represents a number. `x` is a common variable name, but it can just as easily be represented by `y`, `z`, or another name.

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

## Data Types

Now that we know about variables, we can learn about the types of data that a variable can hold. 

A **data type** is a classification of data. Programming languages need to have different data types to interact properly with values. You can do math with a number, but not with a sentence, so the computer classifies them differently. There are six **primitive** (basic) data types: strings, numbers, Boolean, null, undefined, and Symbol (new). Primitives can only hold a single value. Anything that is not one of these primitives is an **Object**. Objects can contain multiple values.

JavaScript is known as a **weakly-typed language** (or *loosely-typed*), which means the language will automatically determine the data type based on the syntax you use. 

## Testing

`alert` and `console.log` are two easy ways to print a value in JavaScript.

```js
var x = 5;

alert(x);
console.log(x);
```

[Here](https://codepen.io/taniarascia/pen/yVgYvx) is a demo of these methods. An `alert` is a popup window and `console.log` will print to the Inspector, which you can find by right-clicking in the browser and selecting **Inspect**. I won't reference these again throughout the article, so you can choose whichever works best for you to practice. I would recommend avoiding the `alert`, as it's very annoying.

You can always find out the type of a variable using `typeof`.

```js
var answer = 42;

typeof answer // returns number
```

### Strings

A **string** is a series of characters.

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

### Numbers

A **number** is a numerical value.

Numbers do not have any special syntax associated with them like strings do. If you were to place a number in quotes (`"5"`), it wouldn't be considered a number, but a character in a string. A number can be whole or a decimal (known as a float), and can have a positive or negative value.

```js
var x = 5; // whole integer
var y = 1.2; // float
var z = -76; // negative whole integer
```

A number can be up to 15 digits.

```js
var largeNumber = 999999999999999; // a valid number
```

You can do regular math with numbers - addition (`+`), subtraction (`-`), division (`/`) and multiplication (`+`).

```js
var sum = 2 + 5; // returns 7
var difference = 6 - 4; // returns 2
```

You can do math with variables.

```js
var elves = 3;
var dwarves = 7;
var men = 9;
var sauron = 1;

var ringsOfPower = elves + dwarves + men + sauron; // returns 20
```

There are two other special number types.

#### NaN

`NaN` means Not a Number, even though it's technically a number type. `NaN` is the result of attempting to do impossible math with other data types.

```js
var nope = 1 / "One"; // returns NaN
```

Attempting to divide a number by a string, for example, results in `NaN`.

#### Infinity

`Infinity` is also technically a number, either the product of dividing by `0` or calculating a number too large.

```js
var beyond = 1 / 0; // returns Infinity
```

### Boolean

A **Boolean** is a value that is either true or false.

Boolean values are very commonly used in programming for when a value might switch between yes and no, on and off, or true and false. Booleans can represent the current state of something that is likely to change.

For example, we'd use a Boolean to indicate whether a checkbox is checked or not.

```js
var isChecked = true;
```

Often, Booleans are used to check if two things are equal, or if the result of a math equation is true or false.

```js
/* Check if 7 is greater than 8 */
7 > 8; // returns false

/* Check if a variable is equal to a string */
var color = "Blue";

color === "Blue"; // returns true
```

> **Note:** A single equals sign (`=`) applies one value to another. A double (`==`) or triple equals sign (`===`) checks if two things are equal.

### Undefined

An **undefined** variable has no value. 

With the `var` keyword, we're *declaring* a variable, but until a value is assigned to it, it's undefined.

```js
var thing; // returns undefined
```

If you don't declare the variable with `var`, it's still undefined.

```js
anotherThing; // returns undefined
```

### Null

**Null** is a value that represents nothing.

Null is the *intentional* absence of any value. It represents something that doesn't exist, and is not any of the other data types. 

```js
var empty = null;
```

The difference between null and undefined is rather subtle, but the main distinction is that null is an intentionally empty value.

### Symbol

A **Symbol** is a unique and immutable data type.

A Symbol is a new primitive data type that emerged with the latest JavaScript release ([ES6](http://www.ecma-international.org/ecma-262/6.0/)). Its main feature is that each Symbol is a completely unique token, unlike other data types which can be overwritten. 

As it is an advanced and little used data type, I won't go into further detail. It is useful to know that it exists, and you can [read more about it here](https://www.sitepoint.com/preparing-ecmascript-6-symbols-uses/).

```js
var sym = Symbol();
```

### Objects

An **object** is a collection of name/value pairs.

Any value that isn't simply a string, number, Boolean, null, undefined, or Symbol is an [object](https://www.sitepoint.com/javascript-object-creation-patterns-best-practises/).

Create an object with a pair of curly braces (`{}`).

```js
var batman = {};
```

Objects consist of **properties** and **methods**. Properties are what the object *is*, and methods are what the object *does*. Returning to the book analogy, properties are like nouns and adjectives, and methods are like verbs.

**Property** | **Method** 
--- | ---
batman.firstName | batman.fight()
batman.location | batman.jump()

We can apply some properties to the `batman` object using name/value pairs (sometimes referred to as *key/value* pairs). They will be comma-separated and written as `propertyName: propertyValue`.

```js
var batman {
  firstName: "Bruce", // string
  lastName: "Wayne", 
  location: "Gotham", 
  introduced: 1939, // number
  billionaire: true, // Boolean
  weakness: null // null
};
```

As you can see, we can apply any primitive data type as a value in an object. We can retrieve an individual value with a dot (`.`).

```js
batman.firstName; // returns Bruce, a string
```

We can also retrieve the value with bracket notation.

```js
batman["firstName"]; // returns Bruce
```

A JavaScript property name must be a valid JavaScript string or numeric literal. If the name begins with a number or has a space, it must be accessed using the bracket notation. [Read: MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Objects_and_properties)

```js
batman.secret identity; // invalid
batman["Secret Identity"]; // valid
```

A method performs an action. Here is a simple example. 

```js
var batman {
  firstName: "Bruce",
  lastName: "Wayne", 
  secretIdentity: function() { // method
    return this.firstName + " " + this.lastName;
  }
};
```

Instead of a simple data type as the value, I have a `function`. The `function` is concatenating `firstName` and `lastName` for `this` object and returning the result. In the example, `this` is the same as `batman` because it's inside the object (`{}`).

```js
batman.secretIdentity(); // returns Bruce Wayne, a concatenation of two properties
```

A method is indicated by parentheses. (`()`).

> **Note:** - the last item in a list of objects does not end in a comma. 

### Arrays

An **array** stores a list into a single variable.

Since an [array](https://www.sitepoint.com/quick-tip-create-manipulate-arrays-in-javascript/) contains more than one value, it's a type of object. Create an array with a pair of straight braces (`[]`).

```js
var ninjaTurtles = [];
```

Arrays do not contain name/value pairs.

```js
var ninjaTurtles = [
  "Leonardo",
  "Michelangelo",
  "Raphael",
  "Donatello"
];
```

You can get an individual value by referencing the `index` of the array. In programming, counting starts at zero, so the first item in a list will always be `[0]`.

```js
var leader = ninjaTurtles[0]; // applies Leonardo to the leader variable
```

You can see how many items are in an array with `length`.

```js
ninjaTurtles.length; // returns 4
```

## Recap

We covered a lot in this article. You should have a better understanding of common programming concepts, terminology, syntax and fundamentals now. At this point, you've learned all about JavaScript data types and variables, and now you're ready to move on to manipulating that data and building programs.  