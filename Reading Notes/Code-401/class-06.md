# Class 06

## Reading

### [How to use Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)

- The random module is a module with a built-in Python method that allows you to generate a random number
- Example: 

      import random
      print random.randint(0, 5)
    
      This will output either 1, 2, 3, 4 or 5.

### [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)

- The probability of any unwanted incident is defined as Risk
- In software Testing, risk analysis is the process of identifying the risks in apps that you built and prioritizing them to test. 
- After that, the process of assigning the level of risk is done
- Use risk analysis to highlight the project's potential problem area's
- Possible risks you may encounter:
        
      Use of new hardware
      Use of new technology
      Use of new automation tool
      The sequence of code
      Availability of test resources for the application

- Certain risks are unavoidable

### [Test Coverage](https://martinfowler.com/bliki/TestCoverage.html)

- Test coverage is a useful tool for finding untested parts of a codebase
- It's not about the quantity more so of how good your tests are
- You're in good shape testing if the following is true:

        You rarely get bugs that escape into production
        You are rarely hesitant to change some code for fear it will cause production bugs.

- If it seems like a simple change to code causes excessively long changes to tests, that's a sign that there's a problem with the tests

## Videos

### [Big O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)

- Rules for describing big O
        
        Different steps get added together
        Drop constants
        Diferent inputs return different variables
        Drop non-dominate terms
        

## Bookmark and Review

### [Python Random](https://docs.python.org/3/library/random.html)

## Further Reading

### [What is Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)

- Dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object.
- A dependency is an object that can be used
- Three types of DI:

        constructor injection: the dependencies are provided through a class constructor.
        setter injection: the client exposes a setter method that the injector uses to inject the dependency.
        interface injection: the dependency provides an injector method that will inject the dependency into any client passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency.
- It's the DI's responsibility to:

        Create the objects
        Know which classes require those objects
        And provide them all those objects
- Benefits of using DI:

        Helps in Unit testing.
        Boiler plate code is reduced, as initializing of dependencies is done by the injector component.
        Extending the application becomes easier.
        Helps to enable loose coupling, which is important in application programming.
- 