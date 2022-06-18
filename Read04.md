[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----
# Reading 04- React and Forms

> What is a ‘Controlled Component’?

- When react controls the state of the component, the form. So we allow react to be the "single source of truth" by controlling the input and output data to the form.

> Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

- No. Set State is slow and we should handle the standard html form states in react. So we should use onChange to keep track of the state in react in real time and then pass the state on submit to the components that need that data.

> How do we target what the user is entering if we have an event handler on an input field?

- we can utilize the event.target.value or we can set the value of the input to a state value and just use a onChange handler to update the local state.


## The Conditional ,Ternary, Operator

> Why would we use a ternary operator?

- Reduce amount of code for if/else statements. Simple one liner that is still easy to read and reduces code required for the same output. 

> Rewrite the following statement using a ternary statement:

- console.log(x===y?true:false);


## Things I want to know more about

- react docs mentioned controlled and uncontrolled. I want to go back and read more about forms and inputs and what the difference really is according to their limited docs.


-----