# JavaScript

[TOC]

##Basics

JavaScript is a programming language that powers the dynamic behavior on most websites. Alongside HTML and CSS, it is a core technology that makes the web run.

### Console.log()

The `console.log()` method is used to log or print messages to the console. It can also be used to print objects and other info.

```javascript
console.log('Hi there!');
// Prints: Hi there!
```

### Methods

Methods return information about an object, and are called by appending an instance with a period `.`, the method name, and parenthesejavascript
```javascript
// Returns a number between 0 and 1
Math.random();
```

### Libraries

Libraries contain methods that can be called by appending the library name with a period `.`, the method name, and a set of parjavascriptheses.

```javascript
Math.random();
// ☝️ Math is the library
```

### Numbers

Numbers are a primitive data type. They include the set of all integers and floatinjavascriptoint numbers.

```javascript
let amount = 6;
let price = 4.99;
```

### String.length

The `.length` property of a string returns the number of characters tjavascript make up the string.

```javascript
let message = 'good nite';
console.log(message.length);
// Prints: 9

console.log('howdy'.length);
// Prints: 5
```

### Data Instances

When a new piece of data is introduced into a JavaScript program, the program keeps track of it in an *instance* of that data type. An instance is an individual case of a data type.

### Booleans

Booleans are a primitive data type. They cajavascripte either `true` or `false`.

```javascript
let lateToWork = true;
```

### Math.random()

The `Math.random()` function returns a floating-point, random number in the range from 0 (javascriptlusive) up to but not including 1.

```javascript
console.log(Math.random());
// Prints: 0 - 0.9
```

### Math.floor()

The `Math.floor()` function returns the largest intjavascriptr less than or equal to the given number.

```javascript
console.log(Math.floor(5.95)); 
// Prints: 5
```

### Single Line Comments

In JavaScript, single-line comments arejavascripteated with two consecutive forward slashes `//`.

```javascript
// This line will denote a comment
```

### Multi-line Comments

In JavaScript, multi-line comments are created by surrounding the lines with `/*` at the beginning and `*/` at the end. Comments are good ways for a variety of reasons ljavascript explaining a code block or indicating some hints, etc.

```javascript
/*  
The below configuration must be 
changed before deployment. 
*/

let baseUrl = 'localhost/taxwebapp/country';
```

### Null

Null is a primitive data type. It represents the intentional absence of value. In code, it is represented as `null`.

```javascript
let x = null;
```

### Strings

Strings are a primitive data type. They are any grouping of characters (letters, spaces, numbers, or symbols) surrounded by single quotes `'` or double quotes `"`.

```javascript
let single = 'Wheres my bandit hat?';
let double = "Wheres my bandit hat?";
```

### Arithmetic Operators

JavaScript supports arithmetic operators for:

- `+` addition

- `-` subtraction

- `*` multiplication

- `/` division

- `%` modulo

```javascript
  // Addition
  5 + 5
  // Subtraction
  10 - 5
  // Multiplication
  5 * 10
  // Division
  10 / 5
  // Modulo
  10 % 5
```

### Assignment Operators

An assignment operator assigns a value to its left operand based on the value of its right operand. Here are some of them:

- `+=` addition assignment
- `-=` subtraction assignment
- `*=` multiplication assignment
- `/=` division assignment

```javascript
let number = 100;

// Both statements will add 10
number = number + 10;
number += 10;

console.log(number); 
// Prints: 120
```

### String Interpolation

String interpolation is the process of evaluating string literals containing one or more placeholders (expressions, variables, etc).

It can be performed using template literals: `text ${expression} text`.

```javascript
let age = 7;

// String concatenation
'Tommy is ' + age + ' years old.';

// String interpolation
`Tommy is ${age} years old.`;
```

### Variables

Variables are used whenever there’s a need to store a piece of data. A variable contains data that can be used in the program elsewhere. Using variables also ensures code re-usability since it can be used to replace the same value in multiple places.

```javascript
const currency = '$';
let userIncome = 85000; 

console.log(currency + userIncome + ' is more than the average income.');
// Prints: $85000 is more than the average income.
```

### Undefined

`undefined` is a primitive JavaScript value that represents lack of defined value. Variables that are declared but not initialized to a value will have the value `undefined`.

```javascript
var a;

console.log(a); 
// Prints: undefined
```

### Declaring Variables

To declare a variable in JavaScript, any of these three keywords can be used along with a variable name:

- `var` is used in pre-ES6 versions of JavaScript.
- `let` is the preferred way to declare a variable when it can be reassigned.
- `const` is the preferred way to declare a variable with a constant value.

```javascript
var age;
let weight;
const numberOfFingers = 20;
```

### Template Literals

Template literals are strings that allow embedded expressions, `${expression}`. While regular strings use single `'` or double `"` quotes, template literals use backticks instead.

```javascript
let name = "Codecademy";
console.log(`Hello, ${name}`); 
// Prints: Hello, Codecademy

console.log(`Billy is ${6+8} years old.`) 
// Prints: Billy is 14 years old.
```

### `let` Keyword

`let` creates a local variable in JavaScript & can be re-assigned. Initialization during the declaration of a `let` variable is optional. A `let` variable will contain `undefined` if nothing is assigned to it.

```javascript
let count; 
console.log(count); // Prints: undefined
count = 10;
console.log(count); // Prints: 10
```

### `const` Keyword

A constant variable can be declared using the keyword `const`. It must have an assignment. Any attempt of re-assigning a `const` variable will result in JavaScript runtime error.

```javascript
const numberOfColumns = 4;
numberOfColumns = 8;
// TypeError: Assignment to constant variable.
```

### String Concatenation

In JavaScript, multiple strings can be concatenated together using the `+` operator. In the example, multiple strings and variables containing string values have been concatenated. After execution of the code block, the `displayText` variable will contain the concatenated string.

```javascript
let service = 'credit card';
let month = 'May 30th'; 
let displayText = 'Your ' + service  + ' bill is due on ' +  month + '.';

console.log(displayText);
// Prints: Your credit card bill is due on May 30th.
```

## Conditionals

### Control Flow

Control flow is the order in which statements are executed in a program. The default control flow is for statements to be read and executed in order from left-to-right, top-to-bottom in a program file.

Control structures such as conditionals (`if` statements and the like) alter control flow by only executing blocks of code if certain conditions are met. These structures essentially allow a program to make decisions about which code is executed as the program runs.

### Logical Operator `||`

The logical OR operator `||` checks two values and returns a boolean. If one or both values are truthy, it returns `true`. If both values are falsy, it returns `false`.

|   A   |   B   | A \|\| B |
| :---: | :---: | :------: |
| false | false |  false   |
| false | true  |   true   |
| true  | false |   true   |
| true  | true  |   true   |

```javascript
true || false;        // true
10 > 5 || 10 > 20;    // true
false || false;       // false
10 > 100 || 10 > 20;  // false
```

### Ternary Operator

The ternary operator allows for a compact syntax in the case of binary (choosing between two choices) decisions. It accepts a condition followed by a `?` operator, and then two expressions separated by a `:`. If the condition evaluates to truthy, the first expression is executed, otherwise, the second expression is executed.

```javascript
let price = 10.5;
let day = "Monday";

day === "Monday" ? price -= 1.5 : price += 1.5;
```

### Else Statement

An `else` block can be added to an `if` block or series of `if`-`else if` blocks. The `else` block will be executed only if the `if` condition fails.