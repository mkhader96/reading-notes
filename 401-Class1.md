# Introduction to Python:

## Reading:
### The Big O Notation
- The link contains a podcast between two developers talking about the Big O notation and how it is used in software development.
- It is a way of evaluating how efficient something is, and it can be used to talk about algorithms and how useful a data structure is based on the algorithm used.
- It means how much time and memory does it take.
- We can think about it as a grade for how efficient something is.
- A+ would be something called constant time, which means that no matter how much data you have, it will always take the same amount of time to run.
- They talk about multiple examples of codes and algorithms and how they are graded based on the Big O notation.

### The Python Environment
- The article goes through the tools and techniques that are used to write and run Python code.
1. The Interpreter
- Pyenv is a set of three tools, from which I present two here, that are pyenv (used to install python) and pyenv-virtualenv (used to configure your global tools).
- The interpreter is the program that reads and executes the code.
2. Dependency Management
- Managing project dependencies in python can become messy or manual. There exists a bunch of tools to help you with that.
- Poetry is a tool that helps you manage your dependencies and your virtual environment.
3. Consistent Formatting and Readability
- Black is a tool for python that allows you to focus on what is necessary, the content. It does that by freeing you from manual code formatting through automation. 
4. Type-Correctness
- Mypy is a static type checker for python code, that finds errors before they appear.
5. Automate the Automation
- Pre-commit is a tool that executes checks before you commit code to your repository (I took for granted that your code is under git version control). When those checks fail, your commit will be rejected. With that, your repository will never see mall formatted code, or none type-checked one, or anything else depending on the checks you are going to include.

### Python 3 Module of the Week
- PyMOTW-3 is a series of articles written by Doug Hellmann to demonstrate how to use the modules of the Python 3 standard library. It is based on the original PyMOTW series, which covered Python 2.7. See About Python Module of the Week for details including the version of Python and tools used.
- It is talking about multiple modules of the Python 3 standard library, and how to use them.
