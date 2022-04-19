# Class 02

## Reading

### [In Tests We Trust - TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

- In Test Driven Development, it's important to write the tests first and then write the functions for the solution you are looking for.

- Tests should be run in their own folders/modules

      mymodule/
        — module.py 
        — another_folder/ 
        — — another_module.py
      tests/ 
        — test_module.py 
        — another_folder/ 
        — — test_another_module.py

- A convention widely used for testing structure is the AAA: Arrange, Act and Assert.

      Arrange: you need to organize the data needed to execute that piece of code (input);

      Act: here you will execute the code being tested (exercise the behaviour)

      Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

- TDD Cycle is made by three steps

      🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right?)

      ✅ Write the feature and make the test pass! 

      🔵 Refactor the code — the first version doesn’t need to be the beautiful one 

- The greatest advantage about TDD is to craft the software design first

- Your code will be more reliable with TDD

### [If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

- With this code you have to comment out the call before using the module by importing it

      def my_function():
        print ("I am inside function")
       <!-- We can test function by calling it. -->
      my_function()

- with this code use main for function call:

      if __name__ == "__main__":
        my_function()

      import myscript

      myscript.my_function()

- Advantages:

    Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

    If you import this script as a module in another script, the __name__ is set to the name of the script/module.

    Python files can act as either reusable modules, or as standalone programs.

    if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

## Videos

### [What on Earth is Recursion](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

- Recursion is a math concept where the incoming argument is an integer variable that has multiple conditions to return multiple values of itself. You need a function stack in order to write it properly

- factorial(n) = n * factorial(n-1)

- The outcome is cascading

## Bookmark and Review

### [Google for Education: Python Lists](https://developers.google.com/edu/python/lists)

### [Google for Education: Python Strings](https://developers.google.com/edu/python/strings)

### [Python Modules and Packages](https://realpython.com/python-modules-packages/)

### [Pytest Documentation](https://docs.pytest.org/en/latest/)

### [PyTest Tutorial](https://www.guru99.com/pytest-tutorial.html)
