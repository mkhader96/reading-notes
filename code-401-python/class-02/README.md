# Introduction to Python:

## Reading:
### In Tests We Trust — TDD with Python
- Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
- TDD:Test-Driven Development is a strategy to think (and write!) tests first.
#### Baby Steps:
- Using the smaller test possible to force yourself to write just enough code for a test to pass.
- The structure:
1. Arrange: you need to organize the data needed to execute that piece of code (input);
2. Act: here you will execute the code being tested (exercise the behaviour);
3. Assert: after executing the code, you will check if the result (output) is the same as you were expecting.
#### The Cycle:
- The cycle is made of three steps:
1. Write a unit test and make it fail;
2. Write the feature and make the test pass;
3. Refactor the code — the first version doesn’t need to be the beautiful one.

### If name equals main
- If the python interpreter is running that module (the source file) as the main program, it sets the special \_\_name__ variable to have a value “\_\_main__”. If this file is being imported from another module, \_\_name__ will be set to the module’s name. Module’s name is available as value to \_\_name__ global variable. 
- The if \_\_name__ == “\_\_main__”: is used to execute the code only when it is invoked directly. The code is not executed when the module is imported.
#### Advantages:
1. Every Python module has it’s \_\_name__ defined and if this is ‘\_\_main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
2. If you import this script as a module in another script, the \_\_name__ is set to the name of the script/module.
3. Python files can act as either reusable modules, or as standalone programs.
4. if \_\_name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

### Recursion
- Recursion is the process in which a function calls itself directly or indirectly
- A recursive function solves a particular problem by calling a copy of itself and solving smaller subproblems of the original problems. Many more recursive calls can be generated as and when required.
#### Properties of Recursion:
1. Performing the same operations multiple times with different inputs.
2. In every step, we try smaller inputs to make the problem smaller.
3. Base condition is needed to stop the recursion otherwise infinite loop will occur.
- Recursion uses more memory, because the recursive function adds to the stack with each recursive call, and keeps the values there until the call is finished. The recursive function uses LIFO (LAST IN FIRST OUT) Structure just like the stack data structure
- Recursion can replace loops, but it is not always the best choice. It is often more efficient to use a loop than to use a recursive function. 

### Python Lists
- A list is a collection which is ordered and changeable. In Python lists are written with square brackets.
-  List literals are written within square brackets [ ]. Lists work similarly to strings -- use the len() function and square brackets [ ] to access data, with the first element at index 0.
- Some of the list methods:
1. append() : Adds an element at the end of the list
2. clear() : Removes all the elements from the list
3. copy() : Returns a copy of the list
4. count() : Returns the number of elements with the specified value
5. extend() : Add the elements of a list (or any iterable), to the end of the current list

### Python Strings
- String literals can be enclosed by either double or single quotes, although single quotes are more commonly used. Backslash escapes work the usual way within both single and double quoted literals.
- A string literal can span multiple lines, but there must be a backslash \ at the end of each line to escape the newline. String literals inside triple quotes, """ or ''', can span multiple lines of text.
- Python strings are "immutable" which means they cannot be changed after they are created (Java strings also use this immutable style). Since strings can't be changed, we construct *new* strings as we go to represent computed values. So for example the expression ('hello' + 'there') takes in the 2 strings 'hello' and 'there' and builds a new string 'hellothere'.
- Some of the most common string methods are:
1. len() - returns the length of a string
2. str() - converts non-string values to strings
3. lower() - converts a string to lowercase
4. upper() - converts a string to uppercase

### Modules and Packages
- Modular programming refers to the process of breaking a large, unwieldy programming task into separate, smaller, more manageable subtasks or modules. Individual modules can then be cobbled together like building blocks to create a larger application.
- Advantages of modular programming:
1. Simplicity
2. Maintainability
3. Reusability
4. Scoping

#### Modules
- The cool thing about modules written in Python is that they are exceedingly straightforward to build. All you need to do is create a file that contains legitimate Python code and then give the file a name with a .py extension.
- The import statement is used to import modules into the current namespace. It allows the programmer to access the functions, objects and variables defined in a module.

#### Packages
- Packages allow for a hierarchical structuring of the module namespace using dot notation. In the same way that modules help avoid collisions between global variable names, packages help avoid collisions between module names.
- A package is a collection of modules. A package is a directory which MUST contain a special file called \_\_init\_\_.py. This file can be empty, and it indicates that the directory it contains is a Python package, so it can be imported the same way a module can be imported.

### PyTest
- PyTest is a testing framework that allows users to write test codes using Python programming language. It helps you to write simple and scalable test cases for databases, APIs, or UI. PyTest is mainly used for writing tests for APIs. It helps to write tests from simple unit tests to complex functional tests.
#### Features:
1. Detailed info on failing assert statements (no need to remember self.assert* names)
2. Auto-discovery of test modules and functions
3. Modular fixtures for managing small or parametrized long-lived test resources
4. Can run unittest (including trial) and nose test suites out of the box
5. Python 3.7+ or PyPy 3
6. Rich plugin architecture, with over 800+ external plugins and thriving community
#### Advantages:
1. Very easy to start with because of its simple and easy syntax.
2. Can run tests in parallel.
3. Can run a specific test or a subset of tests
4. Automatically detect tests
5. Skip tests
6. Open source