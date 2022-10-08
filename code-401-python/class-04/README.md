# FileIO & Exceptions

## Reading:

### Read & Write Files in Python:
#### What is a file?
- A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

#### Files are composed of three main parts:
1. Header: metadata about the contents of the file (file name, size, type, and so on)
2. Data: contents of the file as written by the creator or editor
3. End of file (EOF): special character that indicates the end of the file

#### File Paths:
- To open a file on your computer, you need to know exactly where the file is located. The file patj is three major parts:
1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
2. File Name: the actual name of the file
3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

#### Opening and Closing a File in Python:
1. Open a file: open() function
`open(filename, mode)`
2. Process the file: perform operations on the file
3. Close the file: there are two ways to close a file:
    1. Automatically: using the with statement
    `with open(filename, mode) as file:`
    2. Manually: using the close() method
    `close()`
- Most commonly used file modes:
    - r: read-only mode
    - w: write-only mode
    - rb: read-only mode in binary
    - wb: write-only mode in binary

#### Reading and Writing Opened Files:
- Reading a file:
    - read(): reads the entire file
    - readline(): reads a single line
    - readlines(): reads the entire file line by line into a list
- Writing to a file:
    - write(): writes a string to a file
    - writelines(): writes a list of strings to a file

### Exceptions in Python:
#### What is an exception?
- An exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions.
#### Syntax Errors vs. Exceptions:
- Syntax errors are detected during compilation and are completely unhandled by the program. They are usually easy to detect and fix.
- Exceptions are errors that occur during execution and are not unhandled by the program, i.e. they are not ignored by the program, but handled using the try-except block in Python.

#### Raising an Exception:
- We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.
- The program comes to a halt and displays our exception to screen, offering clues about what went wrong.

#### The AssertionError Exception:
- Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

#### The try and except Block: Handling Exceptions:
- The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

#### The else Clause:
- In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

#### Cleaning Up After Using finally:
- The finally block lets you execute code, regardless of the result of the try- and except blocks.