## Reading and Writing Files in Python (Guide)

What is a file?
- Files on most modern file systems are composed of three main parts:

. Header: metadata about the contents of the file (file name, size, type, and so on)
. Data: contents of the file as written by the creator or editor
. End of file (EOF): special character that indicates the end of the file

File Paths
When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
File Name: the actual name of the file
Extension: the end of the file path pre-pended with a period (.) used to indicate the file type


Opening and Closing a File in Python
- When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:

`file = open('dog_breeds.txt')`

Closing the file:

`reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()`



Character	and their Meaning:
'r'	Open for reading (default)
'w'	Open for writing, truncating (overwriting) the file first
'rb' or 'wb'	Open in binary mode (read/write using byte data)


## Exceptions in Python

Exceptions versus Syntax Errors
- Syntax errors occur when the parser detects an incorrect statement. Observe the following example:

`>>> print( 0 / 0 ))
  File "<stdin>", line 1
    print( 0 / 0 ))`
                  ^
SyntaxError: invalid syntax
The arrow indicates where the parser ran into the syntax error. In this example, there was one bracket too many. 

Raising an Exception
- We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

`x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))`
When you run this code, the output will be the following:

`Traceback (most recent call last):
  File "<input>", line 4, in <module>
Exception: x should not exceed 5. The value of x was: 10`
The program comes to a halt and displays our exception to screen, offering clues about what went wrong.

Key points:
. raise allows you to throw an exception at any time.
. assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
. In the try clause, all statements are executed until an exception is encountered.
. except is used to catch and handle the exception(s) that are encountered in the try clause.
. else lets you code sections that should run only when no exceptions are encountered in the try clause.
. finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

Notes taken from (https://realpython.com/read-write-files-python/#opening-and-closing-a-file-in-python)
(https://realpython.com/python-exceptions/)









