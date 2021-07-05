# Python reference

## Comments and print
```python
# This is a single line comment

"""
This is a multi-line comment
You can write multiple lines
It starts and ends with three double quote characters
"""

print(4) # This sends a value or the result of an expression to the output channel (the server logs, terminal, ...)
# This prints: 4
```

## Basic types and operations

* `int` for integers, this is: non-decimal numbers
* `float` for floating point numbers, this is: decimal numbers with some approximation
* `bool` for boolean, this is True or False
* `string` for text

### Arithmetic operations:

```python
print(1 + 3) # Sum
# This prints: 4

print(3 - 1) # Subtraction
# This prints: 2

print(2 * 3) # Multiplication
# This prints: 6

print(6 / 4) # Division
# This prints: 1.5

print(6 / 2)
# This prints: 3.0

print(3 ** 2) # Exponentiation
# This prints: 9

print(6 // 2) # Integer division (it approximates the value)
# This prints: 3

print(6 // 4)
# This prints: 1

print(-6 // 4)
# This prints: -2
```

### Comparison Operators

```python
print(1 > 3) # Greater than
# This prints: False

print(1 < 3) # Less than
# This prints: True

print(1 <= 3) # Less or equal than
# This prints: True

print(1 >= 3) # Greater or equal than
# This prints: False

print(1 == 5) # Equal to
# This prints: False

print(1 != 3) # Different to
# This prints: True
```

### Logical Operators

```python
print(True and False) # Evaluates if all statements are True
# This prints: False

print(True or False) # Evaluates if at least one of the statements is True
# This prints: True

print(not False) # Flips a boolean value
# This prints: True
```

### Strings

```python
print('This is a string') # String delimited by single quotes
# This prints: This is a string

print("This is also a string") # String delimited by double quotes quotes
# This prints: This is a string

print('This is John\'s string') # Scape string delimiter if it's part of the text
# This prints: This is John's string

print(len('hello')) # String length
# This prints: 5

print('hello' + ' ' + 'world') # String concatenation
# This prints: hello world

greetings = 'Hello'
name = 'John'
print(greetings + ' ' + name) # String concatenation using variables
# This prints: Hello John

print('hello' * 3) # String multiplication
# This prints: hellohellohello

text = 'Hello world'
print(text[0]) # Character at position
# This prints: H
print(text[-1]) # Character at position counting from the end backwards
# This prints: d

print('This is my friend {}'.format('John')) # String substitution
# This prints: This is my friend John

print('This is my friend {name} and he is {age}'.format(age=32, name='John')) # Named string substitution
# This prints: This is my friend John and he is 32

print('I have {money:.2f}€ in my bank account'.format(money=4.1)) # String substitution with fixed decimals
# This prints: I have 4.10€ in my bank account
```

 Complete list of string functions:
* `capitalize()`: Converts the first character to upper case
* `casefold()`: Converts string into lower case
* `center()`: Returns a centered string
* `count()`: Returns the number of times a specified value occurs in a string
* `encode()`: Returns an encoded version of the string
* `endswith()`: Returns true if the string ends with the specified value
* `expandtabs()`: Sets the tab size of the string
* `find()`: Searches the string for a specified value and returns the position of where it was found
* `format()`: Formats specified values in a string
* `format_map()`: Formats specified values in a string
* `index()`: Searches the string for a specified value and returns the position of where it was found
* `isalnum()`: Returns True if all characters in the string are alphanumeric
* `isalpha()`: Returns True if all characters in the string are in the alphabet
* `isdecimal()`: Returns True if all characters in the string are decimals
* `isdigit()`: Returns True if all characters in the string are digits
* `isidentifier()`: Returns True if the string is an identifier
* `islower()`: Returns True if all characters in the string are lower case
* `isnumeric()`: Returns True if all characters in the string are numeric
* `isprintable()`: Returns True if all characters in the string are printable
* `isspace()`: Returns True if all characters in the string are whitespaces
* `istitle()`: Returns True if the string follows the rules of a title
* `isupper()`: Returns True if all characters in the string are upper case
* `join()`: Joins the elements of an iterable to the end of the string
* `ljust()`: Returns a left justified version of the string
* `lower()`: Converts a string into lower case
* `lstrip()`: Returns a left trim version of the string
* `maketrans()`: Returns a translation table to be used in translations
* `partition()`: Returns a tuple where the string is parted into three parts
* `replace()`: Returns a string where a specified value is replaced with a specified value
* `rfind()`: Searches the string for a specified value and returns the last position of where it was found
* `rindex()`: Searches the string for a specified value and returns the last position of where it was found
* `rjust()`: Returns a right justified version of the string
* `rpartition()`: Returns a tuple where the string is parted into three parts
* `rsplit()`: Splits the string at the specified separator, and returns a list
* `rstrip()`: Returns a right trim version of the string
* `split()`: Splits the string at the specified separator, and returns a list
* `splitlines()`: Splits the string at line breaks and returns a list
* `startswith()`: Returns true if the string starts with the specified value
* `strip()`: Returns a trimmed version of the string
* `swapcase()`: Swaps cases, lower case becomes upper case and vice versa
* `title()`: Converts the first character of each word to upper case
* `translate()`: Returns a translated string
* `upper()`: Converts a string into upper case
* `zfill()`: Fills the string with a specified number of 0 values at the beginning

### Variables

```python
this_is_a_number = 123 # Variable names follow snake case format
print(this_is_a_number)
# Prints: 123

weight, height = 70.6, 172.8 # Multiple assignment
print(weight)
# Prints: 70.6
```

### Type and conversion (aka cast)

```python
print(type(3)) # Gets the type of the value/variable
# This prints: <class 'int'>

print(type(3.2)) # Gets the type of the value/variable
# This prints: <class 'float'>

print(type("3")) # Gets the type of the value/variable
# This prints: <class 'str'>

print(type(True)) # Gets the type of the value/variable
# This prints: <class 'bool'>

new_3 = str(3) # Converts to string
print(new_3)
# This prints: 3
print(type(new_3))
# This prints: <class 'str'>

print(float(3)) # Converts int to float
# This prints: 3.0

print(int(3.4)) # Converts float to int
# This prints: 3

print(float('3.4')) # Converts string to float
# This prints: 3.4

print(int('3.4')) # Cannot convert from string to other types if it doesn't follow the expected format
# This prints: Value Error
```

## Data Structures

### Lists

Lists are containers that allow to define **mutable** **ordered** sequence of elements.

```python
week_days = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday'] # List declaration

print(week_days)
# Prints: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']

print(week_days[0]) # Accessing to specific element (index), starting on 0
# Prints: Monday

print(week_days[-1]) # Accessing to specific element (index), starting from the right with negative index
# Prints: Sunday

another_list = [1, False, 3.2, 'four'] # We can declare a list of mixed types
print(another_list)
# Prints: [1, False, 3.2, 'four']

print(week_days[0:5]) # We can get a slice (a portion or sublist) of the list, first number indicates where we start and it's inclusive, the right one where it ends and it's exclusive
# Prints: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday']
print(week_days[5:]) # You don't need to specify the last element if you want the items in the list from the start element
# Prints: ['Saturday', 'Sunday']]
print(week_days[:5]) # Similarly, you don't need to specify the first element if it's the first in the list
# Prints: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday']

print('Saturday' in week_days) # Check if an element is in a list
# Prints: True
print('January' not in week_days) # Check if an element is not in a list
# Prints: False

print(", ".join(week_days))
# Prints: 'Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday'

```

Complete list of string functions:
* `append()`: Adds an element at the end of the list
* `clear()`: Removes all the elements from the list
* `copy()`: Returns a copy of the list
* `count()`: Returns the number of elements with the specified value
* `extend()`: Add the elements of a list (or any iterable), to the end of the current list
* `index()`: Returns the index of the first element with the specified value
* `insert()`: Adds an element at the specified position
* `join()`: Join is a string method that takes a list of strings as an argument, and returns a string consisting of the list elements joined by a separator string.
* `len()`: Returns how many elements are in a list
* `max`: Returns the greatest element of the list. How the greatest element is determined depends on what type objects are in the list. The maximum element in a list of numbers is the largest number. The maximum elements in a list of strings is element that would occur last if the list were sorted alphabetically. This works because the the max function is defined in terms of the greater than comparison operator. The max function is undefined for lists that contain elements from different, incomparable types.
* `min`: Returns the smallest element in a list. min is the opposite of max, which returns the largest element in a list.
* `pop()`: Removes the element at the specified position
* `remove()`: Removes the item with the specified value
* `reverse()`: Reverses the order of the list
* `sort()`: Sorts the list
* `sorted()`: Returns a copy of a list in order from smallest to largest, leaving the list unchanged

### Tuples

Tuples are containers that allow to define an **immutable** **ordered** sequence of elements. They are very usefol for very closely related elements, like X and Y coordinates of a vector.

```python
position = (3, 4)
position2 = 4, 6 # Alternative syntax (can omit the parenthesis)

print("X:", position[0]) # Accessing to an element of the tuple
# Prints: X: 3

x, y = position # Tuple unpacking
print(y)
# Prints: 4
```

### Sets






## References
* [PEP8 - Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)
* [Python official doc](https://docs.python.org/3.9/)
* [HackerRank - Python](https://www.hackerrank.com/domains/python)
* [Codewars - Python](https://www.codewars.com/dashboard)
* [Udacity course](https://classroom.udacity.com/courses/ud1110)
