
1. Svelte 3
2. Ember
3. Vue
4. Angular
5. Ext JS

- technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the flow of the application. You are choosing when and where to call the library. When you use a framework, the framework is in charge of the flow


- JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like



- React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.




- you can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions



- Don’t put quotes around curly braces when embedding a JavaScript expression in an attribute. You should either use quotes (for string values) or curly braces (for expressions), but not both in the same attribute.



- Since JSX is closer to JavaScript than to HTML, React DOM uses camelCase property naming convention instead of HTML attribute names.
For example, class becomes className in JSX, and tabindex becomes tabIndex.


- JSX Prevents Injection Attacks
It is safe to embed user input in JSX:

`const title = response.potentiallyMaliciousInput;
// This is safe:
const element = <h1>{title}</h1>;
`