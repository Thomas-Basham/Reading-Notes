# Class 04

## Reading

### [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

- Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

      class MyClass:
        variable = "blah"

        def function(self):
            print("This is a message inside the class.")
      myobjectx = MyClass()


- To access the variable, use dot notation: myobjectx.variable

- Other things you can do with variables in classes:

      myobjectx = MyClass()
      myobjecty = MyClass()

      myobjecty.variable = "yackity"

- The __init__() function, is a special function that is called when the class is being initiated. It's used for asigning values in a class.


### [Thinking Recursively](https://realpython.com/python-thinking-recursively/)


### [Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

## Bookmark and Review

[Pytest Fixtures](https://docs.pytest.org/en/latest/fixture.html)