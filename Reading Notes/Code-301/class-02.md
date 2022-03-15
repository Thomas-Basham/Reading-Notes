# Readings: State and Props

Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.
Reading.

## [React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

    The Render happens first 

### What is the very first thing to happen in the lifecycle of React?

    The Mounting Phase where the Constructor, static getDerivedStateFromProps,render,componentDidMount, and UNSAFE_componentWillMount occurs

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

    constructor, render, componentDidMount, React Updates, ComponentWillUnmount

### What does componentDidMount do?

    A method for loading anything using a network request or initialize the DOM which is invoked immediately after a component is mounted

## Additional Resources

    [React Bootstrap Documentation](https://react-bootstrap.github.io/)
    [Netlify](https://www.netlify.com/)

## Videos

### [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

### What types of things can you pass in the props?

    Arguments to a function such as object properties

### What is the big difference between props and state?

    Props you pass into the component, state is handled inside of the component. 

    If you're handling information inside of a component and only inside of the component, use state. 
    
    If you're handling that information outside of the component to a parent, use props. 
  
### When do we re-render our application?
  
    When you change the state inside of your application
  
### What are some examples of things that we could store in state?

    Anything the user may enter that will re-render the application such as inputs, settings, forms.

    When you want to change something in your application

## Bookmark/Skim

### [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

### [React Docs - handling events](https://reactjs.org/docs/handling-events.html)

### [React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)
