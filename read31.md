## Why do we not need more .html pages in a multi-page React app?
- because we can render all the content in one page depending on chosed URL.


## If we wanted a component to show up on every page, where would we put it and why?
- Inside the <BrowserRouter />, outside a <Route />

## What does props.children contain?
- whatever included between the opening and closing tags

* **Composition** : It describes a class that references one or more objects of other classes in instance variables

* CHILD COMPONENET: each componenet that is not a root component or serving it.

* Hash routing : A <Router> that uses the hash portion of the URL

# Hooks
- what is a Hook?
Hooks are functions that let you “hook into” React state and lifecycle features from function components
* Hooks let us organize the logic inside a component into reusable isolated units.
*Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

* The main I dea of HOOKS is to apply reusability. Functions seem to be a perfect mechanism for code reuse. Moving logic between functions takes the least amount of effort.
 - However, functions can’t have local React state inside them but there are a soultions for that.. Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

* Each Hook may contain some local state and side effects. You can pass data between multiple Hooks just like you normally do between functions. They can take arguments and return values because they are JavaScript functions.

* **`useState`** returns a pair: the current state value and a function that lets you update it.

* unlike this.state, the state here doesn’t have to be an object 
##### Rules of Hooks:
1. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
2. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks —

* ***Perhaps you’re wondering where React keeps the state for Hooks. The answer is it’s kept in the exact same place where React keeps state for classes. React has an internal update queue which is the source of truth for any state, no matter how you define your components.***

### Main Functions:
1. useState():
  -**EX:** `const [state, setState] = useState(initialState);`
  - the returned state (state) is the same as the value passed as the first argument (initialState).
2. setState():
  - **EX:**  `setState(newState);`
  - The setState function is used to update the state.
3. useEffect(didUpdate);
  - Mutations, subscriptions, timers, logging, and other side effects are not allowed inside the main body of a function component 
  - *But* the useEffect() allow us to do that inside it.
  - will run after the render is committed to the screen.
  - By default, effects run after every completed render, but you can choose to fire them only when certain values have changed.
4. useContext() :
  - `const value = useContext(MyContext);`
  - Accepts a context object (the value returned from React.createContext) and returns the current context value for that context
  - Don’t forget that the argument to useContext must be the context object itself:
    1. Correct: useContext(MyContext)
    2.Incorrect: useContext(MyContext.Consumer)
    3. Incorrect: useContext(MyContext.Provider)
