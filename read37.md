### What is the purpose of a reducer?
- determines changes to an application's state. It uses the action it receives to determine this change

## What does an action contain?
-  a message that we send (i.e. dispatch) to our central Redux store.


## Why do we need to copy the state in a reducer?
- to tell the store theat we creating a new changes because if we didn't it won't read and update on the object asa change


* Immutable state is state that cannot be changed. Immutable objects (for which none of the state can be changed) become important when you are dealing with concurrency, the ability for more than one processor in your computer to operate on that object at the same time.


* *time travel in redux* This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.

 * *action creator* is a plain function that returns an action object


* A **reducer** is a function that determines changes to an application's state.

* *dispatch* is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change.

# multiple Reducers:
- we can create multyiple reducers where each one of them sould has a retrun sstatment

- The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key
-  the updated slices are combined into the new state object.

*higher-order reducer*: which takes an object full of slice reducer functions, and returns a new reducer function.


#### `combineReducers`:
1. combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers.
2. combineReducers enforces several rules to help users avoid common errors.
3. using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.

- There are two ways to define the initial shape and contents of your store's state:
1. First, the createStore function can take `preloadedState` as its second argument. 
2.  The other way is for the root reducer to return the initial state value when the state argument is undefined

- `combineReducrer` will take the whole reducers and make one reducer of them which willl be passed to the `creteStore`