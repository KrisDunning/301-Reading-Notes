[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes/README.html)

-----
# Reading 03- Passing Functions as Props

## React Docs- Lists and Keys

> What does .map() return?

-  .map() returns an array after it is modified by the callback function.

> If I want to loop through an array and display each value in JSX, how do I do that in React?

- wrap each value in curly braces.

> Each list item needs a unique ____.

- key

> What is the purpose of a key?

- to uniquely identify a component so that react can track if it is changed, added or removed.

## The Spread Operator

> What is the spread operator?

- It expands an iterable object into the list of seperate arguments.

> List 4 things that the spread operator can do.

- Copying an array, combining arrays, using the math functions, using an array as arguments.

> Give an example of using the spread operator to combine two arrays.

~~~~~ JS
onst myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
~~~~~

>Give an example of using the spread operator to add a new item to an array.

~~~~~ JS
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

~~~~~

> Give an example of using the spread operator to combine two objects into one.

~~~~~ JS
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
~~~~~

## How to Pass Functions Between Components

> In the video, what is the first step that the developer does to pass functions between components?

- Create the function.

> In your own words, what does the increment function do?

- creates a copy of the people array, which is a state of the App components, and checks to match a name property of the people array. It then increments the count property associated with the person object.Then it returns the updated person object to the copied array. Finally it setState the people array with the value of the copied(updated) array.

> How can you pass a method from a parent component into a child component?

- set the increment function as a prop of the parent component. within the child, we can access the prop and incoke a call to the parent function.

>How does the child component invoke a method that was passed to it from a parent component?

- this.props.`<parent method name>`. We must have a state change to invoke a refresh and that will re-pass props down the chain again. In video he uses a state property of haschanged and sets it to true in the child method. And false in constructor.

## Things I want to know more about

Lifting state up. I saw the additional reading but more experience needed. Also just how is react class vs functional different? need more information on this as well. 

-----