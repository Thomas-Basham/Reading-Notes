# Class-03

## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

### What does .map() return?

    An array

### If I want to loop through an array and display each value in JSX, how do I do that in React?

    You would use the .map() method and then wrap the result in curly braces

    "JSX allows embedding any expression in curly braces so we could inline the map() result:"

### Each list item needs a unique ____

      Key

### What is the purpose of a key?

    To give the elements an identity

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

### What is the spread operator?

    Three dots ... to expand an iterable object into the list of arguments

### List 4 things that the spread operator can do

    Copy an array
    Concatenate or combine arrays
    Using Math functions
    Use an array as arguments
    Add an item to a list
    Add to state in React
    Combine objects
    Converte NodeList to an array

### Give an example of using the spread operator to combine two arrays
  
    const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
  
### Give an example of using the spread operator to add a new item to an array
  
    const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
  
### Give an example of using the spread operator to combine two objects into one

    const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

## Videos

## [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

## In the video, what is the first step that the developer does to pass functions between components?

      Create an function named increment 

## In your own words, what does the increment function do?

    It acts as a counter 

## How can you pass a method from a parent component into a child component?

    methodName={this.methodName} inside of the child component

## How does the child component invoke a method that was passed to it from a parent component?

  this.props.methodName()

## Bookmark/Skim

## [React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)

## [React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)
