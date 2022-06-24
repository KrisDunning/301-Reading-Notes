[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----
# Reading 09- Functional Programming

## Functional Programming Concepts

> What is functional programming?

- A programming style of the structure and elements of programs that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data.

> What is a pure function and how do we know if something is a pure function?

- If it returns the same result if given the same arguments (deterministic) and does not cause any observable side effects. 

> What are the benefits of a pure function?

- They are stable, consistent and predicatable. Easier to test. 

> What is immutability?

- Unchanging over time or unable to change.

> What is Referential transparency?

- replacing a function call with the outcome that is pre-deterministic. Pure functions+immutable date=referential transparency.

## Node.js Modules and Require

> What is a module?

- A module contains code with a logical functionality.

> What does the word ‘require’ do?

- It tells the program that the file(module) is needed to be included.

> How do we bring another module into the file the we are working in?

- module.exports= 'what we want available in the required file'

> What do we have to do to make a module available?

- both require and export the module.



## Things I want to know more about

Is OOP the opposite of functional programming? I know F# is functional based, any other languages that explicitly use functional programming?

-----