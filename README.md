# React Hooks

Hooks were added to React in version 16.8.

Hooks allow function components to have access to state and other React features. Because of this, class components are generally no longer needed.

### Hook Rules
There are 3 rules for hooks:

- Hooks can only be called inside React function components.
- Hooks can only be called at the top level of a component.
- Hooks cannot be conditional.

### React useState Hook
The React useState Hook allows us to track state in a function component.

State generally refers to data or properties that need to be tracking in an application.

#### Import useState
To use the useState Hook, we first need to import it into our component.
```javascript
import { useState } from "react";
```

##### Full code at -> [useState](https://github.com/Anshtripathi079/react_hooks/tree/master/src/components/usestate)
##### Other References -> [w3schools](https://www.w3schools.com/REACT/react_usestate.asp)

### React useEffect Hook
The useEffect Hook allows you to perform side effects in your components.

Some examples of side effects are: fetching data, directly updating the DOM, and timers.

useEffect accepts two arguments. The second argument is optional.
```js
useEffect(<function>, <dependency>)
```
##### Full code at -> [useEffect](https://github.com/Anshtripathi079/react_hooks/tree/master/src/components/useeffect)
##### Other References -> [w3schools](https://www.w3schools.com/REACT/react_useeffect.asp)

### React useContext Hook
React Context is a way to manage state globally.

It can be used together with the useState Hook to share state between deeply nested components more easily than with useState alone.

##### The Problem
State should be held by the highest parent component in the stack that requires access to the state.

To illustrate, we have many nested components. The component at the top and bottom of the stack need access to the state.

To do this without Context, we will need to pass the state as "props" through each nested component. This is called "prop drilling".

##### Full code at -> [useContext](https://github.com/Anshtripathi079/react_hooks/tree/master/src/components/usecontext)
##### Other References -> [w3schools](https://www.w3schools.com/REACT/react_usecontext.asp)

### React useRef Hook
The useRef Hook allows you to persist values between renders.

It can be used to store a mutable value that does not cause a re-render when updated.

It can be used to access a DOM element directly.
#### Does Not Cause Re-renders
If we tried to count how many times our application renders using the useState Hook, we would be caught in an infinite loop since this Hook itself causes a re-render.

To avoid this, we can use the useRef Hook.
##### Full code at -> [useRef](https://github.com/Anshtripathi079/react_hooks/tree/master/src/components/useref)
##### Other References -> [w3schools](https://www.w3schools.com/REACT/react_useref.asp)

### React useReducer Hook
The useReducer Hook is similar to the useState Hook.

It allows for custom state logic.

If you find yourself keeping track of multiple pieces of state that rely on complex logic, useReducer may be useful.

#### Syntax
The useReducer Hook accepts two arguments.
```js
useReducer(<reducer>, <initialState>)
```

The reducer function contains your custom state logic and the initialStatecan be a simple value but generally will contain an object.

The useReducer Hook returns the current state and a dispatchmethod.
##### Full code at -> [useReducer](https://github.com/Anshtripathi079/react_hooks/tree/master/src/components/usereducer)
##### Other References -> [w3schools](https://www.w3schools.com/REACT/react_usereducer.asp)

