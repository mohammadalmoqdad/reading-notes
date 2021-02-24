## Do child components have direct access to props/state from the parent?
- No, That is done by returing the result of the function that had been passed with the props to thge children.

## When a component “wraps” another component, how does the child component’s output get rendered?
- by import it inside the parent class and pass the props object to it.

## Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
- Yes, the componenets themselves are re-usable because they are just a snippet of code. But the thing that should be marked that the correc props chould be passed to it.

## What trick can a parent use to share all props with it’s children
- gater all of them in one componenet and send the values to them.

* **props. children** does is that it is used to display whatever you include between the opening and closing tags when invoking a component.

* **Composition**: it is a natural pattern of the component model. *It's how we build components from other components*, of varying complexity and specialization through props


- Installation: 
`npm i react-router  react-router-dom react-router-native`


- Types of routers:
1. The `<BrowserRouter>` should be used when you have a server that will handle dynamic requests.
2. the `<HashRouter>` should be used for static websites (where the server can only respond to requests for files that it knows about).


- Routes: 
* The `<Route>` component is the main building block of React Router.  
* Anywhere that you want to only render content based on the ***location’s pathname***, you should use a `<Route>` element.