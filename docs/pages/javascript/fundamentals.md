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
6. undefined - undefined – a type with a single value undefined, meaning “not assigned”.
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

**Loops:** In Javascript or any programming language, we have loops. Loops are used to do any repetition task until a condition is fulfilled each time with a different value.

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

- "get…" – return a value,
- "calc…" – calculate something,
- "create…" – create something,
- "check…" – check something and return a boolean, etc.

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
