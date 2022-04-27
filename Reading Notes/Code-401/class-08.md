# Class 08
## Reading

### [List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
- List comprehension is a powerful and concise method for creating lists in Python
- Syntax example:
 
  my_new_list = [ expression for item in list ]
  
  digits = [x for x in range(10)]
      print(digits) # outcome: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
  user_data = "Elvis Presley 987-654-3210"
  <br>
  phone_number = [ x for x in user_data if x.isdigit()]
  print(phone_number) # outcome: ['9', '8', '7', '6', '5', '4', '3', '2', '1', '0']
  <br>

file = open("dreams.txt", 'r')
poem = [ line for line in file ]

for line in poem:
    print(line)
    

## Bookmark and Review

### [Primer on Decorators](https://realpython.com/primer-on-python-decorators/)