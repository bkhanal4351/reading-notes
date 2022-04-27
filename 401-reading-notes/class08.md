## List Comprehensions

Syntax
- Consider the following example:

`my_new_list = [ expression for item in list ]`

1. First is the expression we’d like to carry out. expression inside the square brackets.
2. Second is the object that the expression will work on. item inside the square brackets.
3. Finally, we need an iterable list of objects to build our new list from. list inside the square brackets.


Create a List with range()

Example 1: Creating a list with list comprehensions

 . construct a basic list using range() and list comprehensions
 . syntax
 . [ expression for item in list ]
digits = [x for x in range(10)]

print(digits)
Output

[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

Create a List Using Loops and List Comprehension in Python

Example 2: Comparing list creation methods in Python

First, create a list and loop through it. Add an expression, in this example, we’ll raise x to the power of 2.

 create a list using a for loop
squares = []

`for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)

print(squares)
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]`
Output

Multiplying Parts of a List

Example 3: Multiplication with list comprehensions

`create a list with list comprehensions
multiples_of_three = [ x*3 for x in range(10) ]

print(multiples_of_three)
Output

[0, 3, 6, 9, 12, 15, 18, 21, 24, 27]`


Show the first letter of each word using Python

Example 4: Using list comprehensions with strings

 a list of the names of popular authors
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

 create an acronym from the first letter of the author's names
`letters = [ name[0] for name in authors ]
print(letters)
Output

['E', 'L', 'F', 'T', 'E', 'S']`



Lower/Upper case converter using Python

Example 6: Changing a letter’s case

`lower_case = [ letter.lower() for letter in ['A','B','C'] ]`
`upper_case = [ letter.upper() for letter in ['a','b','c'] ]`

`print(lower_case, upper_case)`
Output

`['a', 'b', 'c'] ['A', 'B', 'C']`

Notes taken from (https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)