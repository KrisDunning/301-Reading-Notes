[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----
# Reading 05- Putting it all together

This relates to our overall project in that it explains how we should think and code in React based on the needs of the product.


## React Docs- Thinking in React

>What is the single responsibility principle and how does it apply to components?

- A component should only do one thing. If a component grows, it should be split into smaller components

>What does it mean to build a ‘static’ version of your application?

- Make your app render the UI and data model but dont use state at all and dont allow interactivity. Components should only have render() methods.

>Once you have a static application, what do you need to add?

- State. State allows us to trigger changes to our underlying data model. 

>What are the three questions you can ask to determine if something is state?

- Is it passed in from a parent via props? If so, it probably isn’t state.
- Does it remain unchanged over time? If so, it probably isn’t state.
- Can you compute it based on any other state or props in your component? If so, it isn’t state.

>How can you identify where state needs to live?

- Identify every component that renders something based on that state.
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.


## Higher Order Functions

>What is a “higher-order function”?

- Functinos that operate on other functions either by taking them as arguments or by returning them.

>Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

- returns a true or false if m is greater than n.

>Explain how either map or reduce operates, with regards to higher-order functions.

-Reduce iterates through an array and apply some logic that results in a single element remaining which then becomes a part of the next logic set until a single element remains.


## Things I want to know more about

reduce. its confusing in its application. or higher order functions in general. 

-----