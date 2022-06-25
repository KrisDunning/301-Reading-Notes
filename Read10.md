[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----
# Reading 10- In Memory Storage



> What is a ‘call’?

- A call is a function invocation

> How many ‘calls’ can happen at once?

- One at a time. Top to bottom. The call stack is synchronous.

> What does LIFO mean?

- Last In, First Out

> Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

- function first(){};
  function second(){first()};
  function third(){second()};
  
  third();

> What causes a Stack Overflow?

- If we hit a recursive functino without a exit point. Eventually we hit a stack call limit and throw an error.

## JavaScript error messages

> What is a ‘reference error’?

- Referencing a variable before it is declared.

> What is a ‘syntax error’?

- When you have something that cannot be parsed in terms of syntax.

> What is a ‘range error’?

- Going beyond a finite distance. Going beyond an array length for example. 

> What is a ‘type error’?

- When the types you are trying to use or access are incompatible. 

> What is a breakpoint?

- A point you can select in your code editor that will pause the code and open the debugger.

> What does the word ‘debugger’ do in your code?

- Same as a breakpoint.


## Things I want to know more about

need more practice using debugger. I hear its good to know call stack in and out but i could use some more review about that. 

-----