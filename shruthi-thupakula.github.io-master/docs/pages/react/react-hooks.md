### React Hooks

React hooks **adds the functionality class components to functional components**.
React supports the following hooks

1. **useState** : Which implements the state functionality of class component.

2. **useEffect** : Implements the changes listener and life cycle methods of class based components.

3. **useLayoutEffect** : Expensive ( works on DOM instead of V-DOM) method which works over useEffect.

- Generally **used to block the execution / Rendering till some actions are done**.

4. **useRef** : Can be used to hold the **DOM element reference** (when component renders, there may be a lose of its original instance in DOM) but using useRef, that can be persistent irrespective of re-renders.

5. **useCallback** : Can be used while updating or calling multiple states at a time. ( as state update or useState is asynchronous, there may be any performance issues as each state change will hit a re-render, use call back will run all of them in parallel and prevents multiple re-renders).

6. **useMemo**: Memoization method for saving calculated efforts for future reference and reduce re-renders and expensive calculations. Majorly used to avoid re-renders even on no props, state change. (alternative of memo(component)).

7. **useContext** : Global state management method, inspired from redux. Which again has same provider (store), consumer pattern with actions, dispatch and reducer (useReducer, useCallback) logic.

Apart from this there are some other hooks which are bound to specific use case and one can write his own hooks using the above.

> **LifeCycle methods with Hooks** :

**Note** : All the LifeCycle methods of class based components can be achieved with useEffect.

useEffect takes 2 parameters,

> useEffect(methodToExecute, dependencyArray).

> useEffect relies on dependency array, which defines when to execute the given method. And that method can also contain a function in return which will be called before the component unMounting or death or removal from DOM.

example:

```JSX
useEffect(()=>{
    console.log(`Hi ${name}`);
    return ()=>{
        console.log(`Bye ${name}`);
    }
},[name])
```

The above useEffect will execute the method each time the parameter "name" changes and return a method or also unknown as executes the returning method when unMounting from dom.
i.e, on name change, it will greet `Hi ${name}` and `Bye ${name}` before unMounting.

1. **Mounting**

   After entering to the dom, ie, componentDidMount implementation can be achieved by useEffect with empty dependency array
   i.e,

   ```JSX
   useEffect(()=>{

   },[]);
   ```

   as there are no dependencies, useEffect will execute the method only once.

   **Note** : Some methods like componentWillMount cannot be directly achieved by useEffect but the useCase can be implemented.

2. **Updating / Rendering**
   As explained above, to listen for changes on a particular prop, we can use useEffect with those parameters in its dependencyArray
   i.e,

   ```JSX
   useEffect(()=>{
       console.log('there is change in param and or or param2');
   }, [param1,param2])
   ```

   as stated, the useEffect will trigger the given method when there is a change in either of dependencies(param1 and param2).

   if the dependencyArray itself is removed ? then useEffect will trigger the given method for each update in component.

   i.e.,

   ```JSX
   useEffect(()=>{
       console.log("something changed");
   })
   ```

   as there is no dependencyArray, each change is caught by the useEffect.

3. **unMounting**
   As explained in one of the statements above, to execute any logic before unMounting the component, we can return any method with the useEffect.

   Note: any useEffect can return a method and all the returning methods will be executed before unMounting itself.

   i.e,

   ```JSX
   useEffect(()=>{
       return ()=>{
           console.log('bye bye from empty dependencyArray');
       }
   },[])
   ```

   ```JSX
   useEffect(()=>{
       return ()=>{
           console.log('bye bye, from useEffect with param1');
       }
   },[param1])
   ```

   ```JSX
   useEffect(()=>{
       return ()=>{
           console.log('bye bye, from all changes listener ');
       }
   })
   ```

   - All of the above methods are valid and will execute the returning methods before unMounting.
     And if above three methods present in one components, all the three consoles statements can be observed while the component is unMounting.

   (**Note**: the order of the execution depends on implementation criteria and is asynchronous, so statements printing may vary based on implementation).
