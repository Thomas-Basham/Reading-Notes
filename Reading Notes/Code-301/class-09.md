# Class 09

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

### What is functional programming?

    Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

### What is a pure function and how do we know if something is a pure function?

    It returns the same result if given the same arguments (it is also referred as deterministic)
    
    It does not cause any observable side effects

### What are the benefits of a pure function?

    Pure functions are stable, consistent, and predictable.
    
### What is immutability?

    Unchanging over time or unable to be changed.

### What is Referential transparency?

    Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

    pure functions + immutable data = referential transparency

## Videos

### [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

### What is a module?

     A block of code put in another file to be used in other files

### What does the word ‘require’ do?

    It imports the file 

### How do we bring another module into the file the we are working in?

 let variable = require('./filename');

### What do we have to do to make a module available?

  module.exports = functionName;
