# Class-04

## [React Docs - Forms](https://reactjs.org/docs/forms.html)

## What is a ‘Controlled Component’?

    A technique for passing a function into an elements value

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why

    It depends on what the type of input is. If it needs validation such as a credit card number to make sure the user's format is right than instant would be good, but if it's a password, instant wouldn't be good because then someone could guess the password easier

## How do we target what the user is entering if we have an event handler on an input field?

    Put an event handler on the onChange event

## [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

## Why would we use a ternary operator?

    To shorten an if statement

## Rewrite the following statement using a ternary statement

    if(x===y){
      console.log(true);
    } else {
      console.log(false);
    }

    x===y ? console.log(true) : console.log(false);

## Bookmark/Skima

    [React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)
    [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)

## Notes

        if ( condition ) {
      value if true;
    } else {
      value if false;
    }

    condition ? value if true : value if false
