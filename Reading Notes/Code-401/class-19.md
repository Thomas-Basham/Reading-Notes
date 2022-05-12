# Class 18
## Reading

### [Python Regular Expressions Tutorial](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)

    Character(s) 	What it does
    . 	A period. Matches any single character except the newline character.
    ^ 	A caret. Matches a pattern at the start of the string.
    \A 	Uppercase A. Matches only at the start of the string.
    $ 	Dollar sign. Matches the end of the string.
    \Z 	Uppercase Z. Matches only at the end of the string.
    [ ] 	Matches the set of characters you specify within it.
    \ 	∙ If the character following the backslash is a recognized escape character, then the special meaning of the term is taken.
    ∙ Else the backslash () is treated like any other character and passed through.
    ∙ It can be used in front of all the metacharacters to remove their special meaning.
    \w 	Lowercase w. Matches any single letter, digit, or underscore.
    \W 	Uppercase W. Matches any character not part of \w (lowercase w).
    \s 	Lowercase s. Matches a single whitespace character like: space, newline, tab, return.
    \S 	Uppercase S. Matches any character not part of \s (lowercase s).
    \d 	Lowercase d. Matches decimal digit 0-9.
    \D 	Uppercase D. Matches any character that is not a decimal digit.
    \t 	Lowercase t. Matches tab.
    \n 	Lowercase n. Matches newline.
    \r 	Lowercase r. Matches return.
    \b 	Lowercase b. Matches only the beginning or end of the word.
    + 	Checks if the preceding character appears one or more times.
    * 	Checks if the preceding character appears zero or more times.
    ? 	∙ Checks if the preceding character appears exactly zero or one time.
    ∙ Specifies a non-greedy version of +, *
    { } 	Checks for an explicit number of times.
    ( ) 	Creates a group when performing matches.
    < > 	Creates a named group when performing matches.

- Common methods working with regex:
  - compile
  - search
  - match
  - findall
  - finditer
  - sub
  - subn
  - start
  - end
  - span

### [shutil](https://pymotw.com/3/shutil/)
- The shutil module includes high-level file operations such as copying and archiving.
- copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.

      import glob
      import shutil

      print('BEFORE:', glob.glob('shutil_copyfile.*'))

      shutil.copyfile('shutil_copyfile.py', 'shutil_copyfile.py.copy')

      print('AFTER:', glob.glob('shutil_copyfile.*'))

## Videos

### [Automation Ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)
- You can use Python to automate tasks like organizing files on your machine,
- opening a browser based on a wide range of conditions
### [Optional: Automating Your Browser and Desktop Apps](https://www.youtube.com/watch?v=dZLyfbSQPXI)
- from selenium import webdriver
- browser = webdriver.Chrome()
- elem = browser.find_element_by_css_selector(copy selector in chrome, paste in here)
- from selenium.webdriver.common.keys import keys
## Bookmark and Review

### [Watchdog](https://pythonhosted.org/watchdog/)