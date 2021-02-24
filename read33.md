## Describe use cases for useMemo() and useReducer()
- With useMemo you can create a value that will be computed from a function you give to the hook and it will change if some of the dependencies in the dependency array changes.
- Use useReducer if you have:
    A) JavaScript objects or arrays as state
    B) complex state transitions
    C) complicated business logic more suitable for a reducer function
    D) different properties tied together that should be managed in one state object
    E) the need to update state deep down in your component tree
    F) a medium-sized application (NB: the lines are blurry here)
    G) need for an easier time testing it
    H) need for a more predictable and maintainable state architecture

## Why do custom hooks need the use prefix?
- The use prefix is just a convention to identify hook functions which are usually call at the very top of a component render method.

## What do custom hooks usually do?
-  custom Hook can return anything as long as the caller knows how to process it.
-   It returns an array in a similar way to how useState does.



# Context:
- When to Use Context?
  * Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- To wrap Updates on the level of the tree, then these updates should be added with the `<APP/>` component to apply it on the whole children.

- If I wanted to will pass the value of the state  wbich has the properties that I want it to be applied on all children 

- does that mean the changing in the main will affect on the chidren component ?
  * No, The children has access to the parent children 

- **Tree**: is simplified concept of the children, root server and the parent component.

- We are:
1. creatig the context element using React.createContext.
2. creating component 
3. creating provider
4. importing the context.
5. assigning values for the context properties.
6. import the provider on the level of the main as a parent for it. 
  - *This is DONE to make te chnages applied inside the whole tree*

- when some data needs to be accessible by many components at different nesting levels.

- There are 4 types of imports for the contexts:
  1. import one context inside class component. 
    - **EX** :`static conteextType = importedContext;` 
  2. import one context inside functions component.
    - **EX**: `const ocntext = useContext(imported context)`
  3. import several contexts inside class component.
    - **EX** :`<MyContext.Consumer> {value => /* render something based on the context value */} </MyContext.Consumer>` 
  4. import several contexts inside functional component.
    - **EX**: `const ocntext = useContext(imported context)`
   


