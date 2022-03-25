# Class 10

## [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

### What is a ‘call’?

    Function invocation

### How many ‘calls’ can happen at once?

    one call at a time

### What does LIFO mean?

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack

    function firstFunction(){
      console.log("Hello from firstFunction");
    }

    function secondFunction(){
      firstFunction();
      console.log("The end from secondFunction");
    }

    secondFunction();

### What causes a Stack Overflow?

    A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

    Here is an example:

    function callMyself(){
      callMyself();
    }

    callMyself();

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

### What is a ‘refrence error’?

when you try to use a variable that is not yet declared you get this type os errors.

### What is a ‘syntax error’?

this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

### What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up

### What is a ‘type error’?

Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

### What is a breakpoint?

Used for debugging, will make your code run as long as a condition is met in breakpoint

### What does the word ‘debugger’ do in your code?

it tests your code and shows return in the "local" tab

## [Additional Resources](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

### JavaScript errors reference on MDN
