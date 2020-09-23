### React Basics

React is a front-end JavaScript library.It enhances application performance while allowing for working on both client-side and server-side.Writing UI test cases is simple with React, which is also easy to integrate with other JS frameworks. Excellent for developing web and mobile UI.component-based approach and helps in building reusable UI components. use of the virtual DOM instead of the real DOM. server-side rendering. Supports unidirectional data flow.It supports one way data binding.
In React, everything is a component-it is divisible into a number of small independent and reusable components
by reducing the re-renders we can optimize the react.

State- States are the source of data for React components.state is a object. it determines components behavior and rendering. state is mutable and creates dynamic and interactive components.

Props- Props are inputs to components. They are single values or objects containing a set of values that are passed to components. props are passed down from the parent components to the child components.

Difference between state and props-- Props get passed to the component similar to function parameters whereas state is managed within the component similar to variables declared within a function.
The parent component can change the value in Props but not in the state.
The changes can be made inside the state but not in Props.

Stateful component--A Stateful component stores the change in memory to React. It has the authority to change state and contains vital information of past, current, and future changes.

render( )-- In React, each component must have a render() function. It returns a single React element, which is, in fact, the representation of the native DOM component.

Virtual DOM-- A virtual DOM is a lightweight JS object. It is simply a copy of the real DOM. A virtual DOM is a node tree that lists various elements, their attributes, and content as objects and their properties.
1.its re-rendered when any data changes in UI 2. compare the previous DOM representation and the new one.data changes are calculated.
3.after the calculations ,the real DOM updated with only changes

Real DOM-- supports a very expensive DOM manipulation. Virtual DOM-- inexpensive DOM manipulation.--it updates JSX.-- no memory wastage and updates fast.It cant update HTML directly

controlled components-- which can maintain their state, and their data is controlled by parent component.
uncontrolled components-- which can maintain their state, and their data is controlled by DOM.
Higher-Order Component-- It is an advanced way of reusing the component logic, which wraps another component along with it.
benefits--Reuse of Code, Offers a high hacking facility, Supports state abstraction and manipulation, It offers props manipulation

Pure components -- This component doesn't have any state (irrespective of type (class/functional) they are, they purely depend on parent component called render props. ▪ So if any pure component is rendered then its sure that some props sent by parent are changed.
it include the components which are simple and easy to be written. They can easily replace any component which as a render().

We need a Router to React so that we could define the multiple routes whenever the user types a particular URL.

Functional Components cannot have state and depends on the parent component for data to render and are lite weight ( class components are heavy in terms of memory as they hold this object)
But when hooks came into the picture, it changed the situation as it gave same power of class component to functional component with useState, useEffect etc..
