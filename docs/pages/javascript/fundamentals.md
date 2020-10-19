## Variables

- Variables are used to store the information.
- Name location of memory.
- We can declare variables to store data by using the var, let and const keywords.

1. **const** \- Const variable can only be declared once and at that time of declaration it should be initialized\.

**Example**

`const a='Hello!'`;

- We can't modify or redeclare the **a** value.

2. **let** \- It's value can be modified but it's declaration should be only one time\.

**Example**

```javascript
let a = "Hi";

a = "Hello!";

a = "World!"; //value changed
```

- let **a** can only be given once but a value can be modified any time.

3. **var** \- It has both capabilities \, we can redeclare it and change the value at any time\.

**var**-global scope

**let & const**-blocked scope
<br>

A variable name can include:

- Letters and digits, but the first character may not be a digit.
- Characters \$ and \_ are normal, on par with letters.

###### Data Types

There are  8 basic data types in JS.

```javascript
1. number - for both floating-point and integer numbers.
2. bigint - for integer numbers of arbitrary length.
3. string - for strings.
4. boolean - for logical values: true/false.
5. null - a type with a single value null, meaning “empty” or “does not exist”.
6. undefined – a type with a single value undefined, meaning “not assigned”.
7. object and symbol - for complex data structures and unique identifiers.
```

And `typeof` operator allows us to see which type is stored in a variable.
<br>

###### Interaction: alert, prompt, confirm

**alert**  -  shows a message

```javascript
alert(message);
```

**prompt**  -  shows a message asking the user to input text. It returns the text or, if _Cancel_ button is clicked.

```javascript
prompt(question, [default])
```

**confirm**  -  shows a message and waits for the user to press _OK_ or _Cancel_. It returns true for _OK_ and false for _Cancel_

```javascript
confirm(question);
```

- Ask a question and suggest to choose between Ok and Cancel. The choice is returned as true/false.

**JavaScript strings :**

- JavaScript strings are primitive values. JavaScript strings are also immutable.

1. **Getting the length of the string**

The length property returns the length of a string:

```javascript
let str = "Good Morning!";
console.log(str.length); // 13
```

2. **Accessing characters**

To access the characters in a string, you use the array-like [] notation with the zero-based index.

```javascript
let str = "Hello";
console.log(str[0]); // "H"
```

3. **Concatenating strings**
   To concatenate two or more strings you use the concat().

```javascript
let firstName = "John";
let fullName = firstName.concat(" ", "Doe");
console.log(fullName); // "John Doe"
```

4. **Removing whitespace characters**

To remove all leading whitespace characters of a string, you use the trim().

```javascript
let rawString = " Hi  ";
let strippedString = rawString.trim();
console.log(strippedString); // "Hi"
```

5. **Changing cases**

To change cases of a string, you use toLowerCase() and toUpperCase() methods.

6. **Replacing substrings**

To replace a substring in a string, you use the replace() method.

### **Loops:**

In Javascript or any programming language, we have loops. Loops are used to do any repetition task until a condition is fulfilled each time with a different value.

- three types of loops:

```javascript
// 1
while (condition) {
  ...
}

// 2
do {
  ...
} while (condition);

// 3
for(let i = 0; i < 10; i++) {
  ...
}
```

**switch statement:** The “switch” construct can replace multiple if checks. It uses === (strict equality) for comparisons.

```javascript
switch(x) {
  case 'value1':  // if (x === 'value1')
    ...
    [break]

  case 'value2':  // if (x === 'value2')
    ...
    [break]

  default:
    ...
    [break]
}
```

## Functions

- JavaScript functions that allow you to structure your code into smaller and more reusable units.
- To avoid repeating the same code all over places, you can use a function to wrap that code and reuse it.

###### Function Declaration

- To declare a function, use the function keyword,a list of parameters,and the function body as follows:

```javascript
// Function Declaration
function sum(a, b) {
  return a + b;
}
```

- Function Declarations are processed before the code block is executed. They are visible everywhere in the block.

```javascript
// Function Expression
let sum = function (a, b) {
  return a + b;
};
```

- Function Expression: a function, created inside an expression or inside another syntax construct. Here, the function is created at the right side of the “assignment expression” = :

- Function Expressions are created when the execution flow reaches them.

**Local Variable -** A variable declared inside a function is only visible inside that function.

**Outer Variables -** The function has full access to the outer variable. It can modify it as well.

**Function starting with…**

- `get…` – return a value,
- `calc…` – calculate something,
- `create…` – create something,
- `check…` – check something and return a boolean, etc.

**Arrow Functions -** There’s another very simple syntax for creating functions, that’s often better than Function Expressions.It’s called “arrow functions”, because it looks like this:

?>let func = (arg1, arg2, ...argN) => expression

**Example :**

```javascript
let sum = (a, b) => a + b;
```

**Multiline arrow functions:**

- **(...args) => { body }** – brackets allow us to write multiple statements inside the function, but we need an explicit _return_ to return something.

```javascript
let sum = (a, b) => {
  // the curly brace opens a multiline function
  let result = a + b;
  return result; // if we use curly braces, then we need an explicit "return"
};
```

## Objects

In JavaScript, almost everything is an object.

- Booleans,Numbers and Strings can be objects (if defined with the new keyword).
- Dates are always objects.It stores the information about the date and time.
- Arrays are always objects.It stores the ordered data collections.
- Maths,Regular expressions,Functions and Objects are always objects.
- All JavaScript values, except primitives, are objects.

##### Object Properties:

Object stores the properties (key-value pairs), where:

- Property `keys` must be strings or symbols (usually strings) and `values` can be of any type.
- To access a property, we can use:
  - The dot notation: `obj.property`
  - Square brackets notation `obj["property"]`. Square brackets allow to take the key from a variable, like `obj[varWithKey]`.
- Properties can usually be changed, added, and deleted, but some are read only.

  - To delete a property: `delete obj.prop`

- There are two kinds of object properties.

1. Data properties

The data property sets or returns the value of the data attribute of an <object> element.
The data attribute specifies the URL of the resource to be used by the object.

2. Accessor properties

- Accessor properties are represented by “getter” and “setter” methods.
  - Getters give you a way to define a property of an object, but they do not calculate the property's value until it is accessed.
  - Setter can be used to execute a function whenever a specified property is attempted to be changed.
- In an object literal they are denoted by `get` and `set`.
  - `get` – a function without arguments, that works when a property is read.
  - `set` – a function with one argument, that is called when the property is set.

```javascript
let obj = {
  get propName() {
    // getter, the code executed on getting obj.propName
  },

  set propName(value) {
    // setter, the code executed on setting obj.propName = value
  },
};
```

**Example:**

```javascript
let user = {
  name: "John",
  surname: "Smith",

  get fullName() {
    return `${this.name} ${this.surname}`;
  },

  set fullName(value) {
    [this.name, this.surname] = value.split(" ");
  },
};

// set fullName is executed with the given value.
user.fullName = "Alice Cooper";

alert(user.name); // Alice
alert(user.surname); // Cooper
```

###### Advantages of using Getters and Setters:

- It gives simpler syntax.
- It allows equal syntax for properties and methods.
- It can secure better data quality.
- It can securing access to data properties and adding extra logic to properties before getting or setting their values.

##### Object Methods:

- Functions that are stored in object properties are called “methods”.
- Methods are functions stored as object properties.
- Methods can reference the object as `this`. To access the object, a method can use the `this` keyword.
- When a function is called in the “method”,syntax is `object.method()`,the value of `this` during the call is object.
- In Arrow functions we don't have `this`. When this is accessed inside an arrow function, it is taken from outside.

##### Constructor function:

Constructor functions technically are regular functions. There are two conventions though:

1. They are named with capital letter first.
2. They should be executed only with `new` operator.

**Object Prototypes:** All JavaScript objects inherit properties and methods from a prototype:
`Object.prototype`
