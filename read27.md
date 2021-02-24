### Does a deployed React application require a server?
- No, and the building of the app that is happening is just to get the new changes on the react app.


### Why do we prefer to test a React application at the behavior rather than the unit level?
- 


### What does `npm run build` do?
- will create an optimized build of the app in the ***build*** folder.


### Describe the actual composition / architecture of a React application.
- we can use the composition to create a nav bar or side bar list etc... 




* behavior-driven development (BDD) is an Agile software development process that encourages collaboration among developers.


* Acceptance Testing: This is a type of testing done by users, customers, or other authorised entities to determine application/software needs and business processes. Description: Acceptance testing is the most important phase of testing as this decides whether the client approves the application/software or not.


* Mounting : process where operating system must make it accessible through the computer's file system




# SetState:
- setState() is the only legitimate way to update state after the initial state setup.


- *Reconciliation*: . The reconciliation process is the way React updates the DOM, by making changes to the component based on the change in state. 


* The reconciliation process does not necessarily change the entire tree, except in a situation where the root of the tree is changed


# Handling events :
- The react is giving the ability to response to events using built in reserved words that perform the events. To handle that event it also giver the ability to write whatever the handling will do either inside a function or directly inside the event reserved word.


# Components and Props
* Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.


* The defining of the components is a property that has been added in *`ES6`*


* elements can also represent user-defined components:
  - EX: `const element = <Welcome name="Sara" />;`


-  Props Object : a single bject that has some properities and it is used to pass darta from commponent to another.
* **Props are Read-Only**



# RTL Testing :
* **The more your tests resemble the way your software is used, the more confidence they can give you.**
- findByText is asynchronous! If you forget the await statement a little bit too much, I encourage you to install the following plugin: ***eslint-plugin-testing-library***. It contains a rule that prevent you from doing so! 





