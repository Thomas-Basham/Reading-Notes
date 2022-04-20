# Class 03

## Reading

### [Read & Write Files in Python](https://realpython.com/read-write-files-python/)

- At its core, a file is a contiguous set of bytes used to store data.

- Files on most modern file systems are composed of three main parts:

      Header: metadata about the contents of the file (file name, size, type, and so on)
      
      Data: contents of the file as written by the creator or editor
      
      End of file (EOF): special character that indicates the end of the file

- open is a built in function in python to open files:

      file = open('dog_breeds.txt')

- Make sure to close any files you've opened your code

      reader = open('dog_breeds.txt')
      try:
        # Further file processing goes here
      finally:
        reader.close()

- There are three different categories of file objects:

      Text files
      Buffered binary files
      Raw binary files

- Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met.

- If the condition turns out to be False, you can have the program throw an AssertionError exception.

### [Exceptions in Python](https://realpython.com/python-exceptions/)

- A Python program will run until there is an error

- There are syntax errors and there are exception errors

- You can use raise to throw an exception if a condition occurs

      x = 10
      if x > 5:
          raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

- Try and except blocks work like you would expect:

      try:
          linux_interaction()
      except AssertionError as error:
          print(error)
      else:
          try:
              with open('file.log') as file:
                  read_data = file.read()
          except FileNotFoundError as fnf_error:
              print(fnf_error)
      finally:
          print('Cleaning up, irrespective of any exceptions.')

## Videos

[Read & Write Files in Python - Companion Video](https://realpython.com/courses/reading-and-writing-files-python/)

- Ensure files close by making a try finally block. close file in finally

## Bookmark and Review

[Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)
