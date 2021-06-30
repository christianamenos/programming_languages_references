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

## Arithmetic operations:

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

## Comparison Operators

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

## Logical Operators

```python
print(True and False) # Evaluates if all statements are True
# This prints: False

print(True or False) # Evaluates if at least one of the statements is True
# This prints: True

print(not False) # Flips a boolean value
# This prints: True
```

## Strings

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

## Variables

```python
this_is_a_number = 123 # Variable names follow snake case format
```

## References
* [PEP8 - Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)
