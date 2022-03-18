. What is the single responsibility principle and how does it apply to components?
- The single responsibility principle in JavaScript deals with the cohesiveness of modules. It states that functions and classes should only have one job.

. What does it mean to build a ‘static’ version of your application?
- A version of your app that takes data model and renders UI but has no interactivity.

. Once you have a static application, what do you need to add?
- To make app interactive, we will need to be able to trigger changes to our underlying data model using state from react.

. What are the three questions you can ask to determine if something is state?
- 1. Is it passed in from a parent via props? If so, it probably isn’t state.

2. Does it remain unchanged over time? If so, it probably isn’t state.

3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

. How can you identify where state needs to live?
- 
  . Identify every component that renders something based on that state.
  . Find a common owner component (a single component above all the components that need the state in the hierarchy).
  . Either the common owner or another component higher up in the hierarchy should own the state.
  . If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

  . What is a “higher-order function”?
  - Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

  . Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
  - it is returning another function.



Notes taken from: (https://reactjs.org/docs/thinking-in-react.html)
(https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)



