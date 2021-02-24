## Can a parent component access the state of a child component?
- Yes

## What can be passed along in a prop variable?
- Anything, but usually we pass things from the state object

## How can a child component “know” the state of another component?
- Using the props object.


* **Component Props** are arguments passed into React components. Props are passed to components via HTML attributes.

* **Componenet State** : an object that determines how that component renders & behaves. In other words, “state” is what allows you to create components that are dynamic and interactive.

* **Component state** is the interface between your data from any kind of backend or local change and the representation of this data with UI-elements in the frontend. State is able to keep the data of different components in sync because each state update will rerender all relevant components.


# react basics recap:
- The lifecycle of the commponenet is summerized by :
1. Mounting:
   - the first method that runs is the constructor method. Typically, the `constructor` is where you would initialize component state.  
   - `render` method which returns your JSX. Now React “mounts” onto the DOM.
   - `componentDidMount` method runs. Here is where you would do any ***asynchronous calls*** to databases or directly manipulate the DOM if you need. Just like that, 

2. Updating:
 - This phase is triggered every time state or props change. 
 - No constrcor this Time.
 - **`shouldComponentUpdate`** :
   -  Here you can compare old props/state with the new set of props/state.
   - You can determine if your component should re-render or not by returning true or false
   - If `shouldComponentUpdate` returns false, this update cycle ends.
 - `componentDidUpdate` Method: is hhe place where anyone can add the async calls
 - It keeps updating until it is being removed from the *Virtula DOm*

3. Unmounting:
- `componentWillUnmount` function is run before the component is being removed.
-  ***You should use this method to clean up any open connections such as WebSockets or intervals.***
- Is the removing process for the component form the *Virtual Dom*.

* `forceUpdate` is a method that directly causes a re-render
* A component can only be in one stage at a time.

##### Higher-Order Component:
- is a function that takes a component and returns a new component.
- EX: `const hoc = connect(state => state)const WrappedComponent = hoc(SomeComponent)`
- **What’s the point of passing a function instead of an object?**
  * Because setState is asynchronous, relying on it to create our new value will have some pitfalls. For example, by the time setState runs, another setState could have mutated state. Passing setState a function gives us two benefits. The first is it allows us to take a static copy of our state that will never change on its own. The second is that it will queue the setState calls so they run in order.

# props.children:
- this.props.children does is that it is used to display whatever you include between the opening and closing tags when invoking a component

# React Router v4
- **React Router v4** is a pure React rewrite of the popular React package. Previous versions of React Router used configuration disguised as pseudo-components and could be difficult to understand. 


# Composition vs Inheritance

* React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.

* We can define the props in sevral ways :
  1. props.children: is to send the elements themselves only.
  
  2. adding a name for thje object and sen tags(elements) inside of it.
    - EX: `function App() {
  return (
    <SplitPane
      left={
        <Contacts />
      }
      right={
        <Chat />
      } />
  );
}`

  3. Adding children of another content and assign the values of them inside another component:
  - EX:
  `function Dialog(props) {
  return (
    <FancyBorder color="blue">
      <h1 className="Dialog-title">
        {props.title}
      </h1>
      <p className="Dialog-message">
        {props.message}
      </p>
    </FancyBorder>
  );
}

function WelcomeDialog() {
  return (
    <Dialog
      title="Welcome"
      message="Thank you for visiting our spacecraft!" />
  );
}`


