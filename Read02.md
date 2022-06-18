[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----

# Read 02 - State and Props

## Reading Q & A

- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
  - Render first.

- What is the very first thing to happen in the lifecycle of React?
  - Constructor

- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
  - Constructor, Render, React Updates, ComponentDidMount, ComponentWillUnmount

- What does componentDidMount do?
  - It invokes immediately after a component is mounted. This is a good spot to load anything using a network request or set up subscriptions.

## Video Q & A

- What types of things can you pass in the props?
  - Anything you want to pass to the component. Like arguments to a function. Things to initilize the component.
- What is the big difference between props and state?
  - Props are passed into a component from outside. State is only handled within the component, not outside.
- When do we re-render our application?
  - When we change the state in the component.
- What are some examples of things that we could store in state?
  - Counters, things that a user changes so we can re-render, like form data.

## Things I want to know more about

- Pass state as props? Do we just save the state data in a variable and return it to parent to be passed as a prop?

-----