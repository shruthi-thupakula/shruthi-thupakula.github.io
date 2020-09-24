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

###### Data Types

There are  8 basic data types in JS.

1. number
2. int
3. string
4. boolean
5. null
6. undefined
7. object
8. symbol

And `typeof` operator allows us to see which type is stored in a variable.
<br>

###### Interaction: alert, prompt, confirm

**alert**  -  shows a message

**prompt**  -  shows a message asking the user to input text. It returns the text or, if _Cancel_ button is clicked.

**confirm**  -  shows a message and waits for the user to press _OK_ or _Cancel_. It returns true for _OK_ and false for _Cancel_
<br>

## Functions

- JavaScript functions that allow you to structure your code into smaller and more reusable units.
- To avoid repeating the same code all over places, you can use a function to wrap that code and reuse it.

###### Function Declaration

To declare a function, use the function keyword,a list of parameters,and the function body as follows:

```javascript
function showMessage(parameters) {
  console.log("Hello everyone!");
}
```
