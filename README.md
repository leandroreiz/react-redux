# Redux

## What is Redux?

Redux is a pattern and library for managing and updating application state, using events called "actions". It serves as a centralized store for state that needs to be used across your entire application, with rules ensuring that the state can only be updated in a predictable fashion.

## Action, Reducers and Store

**Actions** are objects that have 2 properties, type and payload.

The **Reducers** are functions that receives the state and action object, decides how to update the state if necessary and returns the new state.

```javascript
(state, action) => newState;
```

You can think of a reducer as an event listener which handles events based on the received action (event) type.

The **Store** is an object where the current Redux application state lives.
