### React Basics

- React is a front-end JavaScript library.It enhances application performance while allowing for working on both client-side and server-side.Writing UI test cases is simple with React, which is also easy to integrate with other JS frameworks. Excellent for developing web and mobile UI.
- Component-based approach and helps in building reusable UI components. use of the virtual DOM instead of the real DOM. server-side rendering. Supports unidirectional data flow.It supports one way data binding.
- In React, everything is a component-it is divisible into a number of small independent and reusable components
- by reducing the re-renders we can optimize the react.

**Virtual DOM**- A virtual DOM is a lightweight JS object. It is simply a copy of the real DOM. A virtual DOM is a node tree that lists various elements, their attributes, and content as objects and their properties.

1. its re-rendered when any data changes in UI
2. compare the previous DOM representation and the new one.data changes are calculated.
3. after the calculations ,the real DOM updated with only changes

**Real DOM**- supports a very expensive DOM manipulation. Virtual DOM-- inexpensive DOM manipulation.--it updates JSX.-- no memory wastage and updates fast.It cant update HTML directly

**render( )**- In React, each component must have a render() function. It returns a single React element, which is, in fact, the representation of the native DOM component.

**State**- States are the source of data for React components.state is a object. it determines components behavior and rendering. state is mutable and creates dynamic and interactive components.

**Props**- Props are inputs to components. They are single values or objects containing a set of values that are passed to components. props are passed down from the parent components to the child components.

- Difference between **state and props** - Props get passed to the component similar to function parameters whereas state is managed within the component similar to variables declared within a function.
  The parent component can change the value in Props but not in the state.
  The changes can be made inside the state but not in Props.

- React has two types of components

1. Class components
2. Functional components

**Class Components**- Class Components holds better state handling as it has a capability of "this" object life cycle methods.

**Functional Component**- Functional Component cannot have state and depends on the parent component for data to render and are lite weight ( class components are heavy in terms of memory as they hold this object)

- Functional Components are pure functions that may return a JSX element.
- But when _hooks_ came into the picture, it changed the situation as it gave same power of class component to functional component with _useState, useEffect_ etc..

> **LifeCycle methods: For the class components**

1. **Mounting**

- First time entering into dom, initialization is called as Mounting.

- **componentWillMount** : the state that is called before
- **render** : initial render
- **componentDidMount**: This methods gets called only once after component birth.

2. **Updating / Rendering**

- When there is change in props or state, react will kick a new render, that is called as updating.
- **componentWillReceiveProps** : the method called before receiving props
- **componentWillUpdate** : method called before the update

- **shouldComponentUpdate** ( if yes, next step will be taken ) : Boolean method to confirm whether to render or not?
- **render** -**componentDidUpdate** : method called after the update/render

3. **UnMounting**

- The last stage of the component.

- **componentWillUnMount**: this method gets called before removing the component from DOM. Generally this method is used to reset any details saved that are no longer needed.

**Stateful component**- A Stateful component stores the change in memory to React. It has the authority to change state and contains vital information of past, current, and future changes.

- The components that have local state management, or self state.

**Stateless Components** : The components that completely relies on the parent component for its data and is purely driven by render props.

**Pure components**- This component doesn't have any state (irrespective of type (class/functional) they are, they purely depend on parent component called render props.

- So if any pure component is rendered then its sure that some props sent by parent are changed.
  it include the components which are simple and easy to be written. They can easily replace any component which as a render().

**Note** : Pure Components are the components that implement shouldComponentUpdate method by default, which will prevent unwanted re-renders.

**Controlled components**- which can maintain their state, and their data is controlled by parent component.

**Uncontrolled components**- which can maintain their state, and their data is controlled by DOM.

**Higher-Order Component**- It is an advanced way of reusing the component logic, which wraps another component along with it.
**benefits**- Reuse of Code, Offers a high hacking facility, Supports state abstraction and manipulation, It offers props manipulation

We need a **Router to React** so that we could define the multiple routes whenever the user types a particular URL.
