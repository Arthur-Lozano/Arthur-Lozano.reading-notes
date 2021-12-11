

# Read and write files in python

> One of the most common tasks that you can do with Python is reading and writing files. Whether it’s writing to a simple text file, reading a complicated server log, or even analyzing raw byte data, all of these situations require reading or writing a file.
- (..) can be chained together to move across multiple directories above the current directory.
- To open a file : file = open('dog_breeds.txt') Note: always ensure an open file is properly closed
-File types
* Text File Types - the most common file that we work with.
* Buffered binary file types are use for reading and writing binary files.
* Raw Files - Usually used as a low-level building block for binary and text streams.
- How to read an entire file as a list using the Python .readlines()
- f = open('dog_breeds.txt')\n list(f)

# Exceptions in python

- A python program terminates as soon as it encounters an error
- Two types of erros in Python
* Syntax error
* exception 
- Exceptions vs syntax errors
* Syntax errors happen when the parser detects an incorrect statement.
- The arrow indicates where the parser ran into the syntax error.
* Exception errors ocur whenever code is syntactically correct 
* Python  details the type of exception error was found such as (ZeroDivisionError) Instead of a plain exception error
* raise - if you want to throw an error when a certain condition will occur
* The (try and except) Block is used for handling exceptions
* With Python using the else statement one can instruct a program to execute a certain block of code only in the absence of exceptions.

### References

* https://realpython.com/read-write-files-python/
* https://realpython.com/python-exceptions/