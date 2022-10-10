# Intro to OOP

## Reading:

### Classes and Objects:
- Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes.
- Classes are essentially a template to create your objects.
- init() : The __init__() function, is a special function that is called when the class is being initiated. It's used for assigning values in a class.

### Thinking Recursively:
- A recursive function is a function defined in terms of itself via self-referential expressions.
- Each recursive call has its own execution context, so to maintain state during recursion you have to either:
1. Thread the state through each recursive call so that the current state is part of the current call’s execution context
2. Keep the state in global scope

- Recursive Data Structures in Python: A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure.

### Pytest Fixtures and Coverage:
- Fixtures are functions, which will run before each test function to which it is applied. Fixtures are used to feed some data to the tests such as database connections, URLs to test and some sort of input data. Therefore, instead of running the same code for every test, we can attach fixture function to the tests and it will run and return the data to the test before executing each test.
- Coverage: report for every part of the Python library that your program used, so I strongly suggest you provide an argument to --cov, specifying which program(s) you want to test. And, you should indicate the directory into which the report should be written.

- To install the coverage tools
`python -m pip install pytest-cov`
- To run the coverage command:
`pytest --cov blackjack --cov-report html`

