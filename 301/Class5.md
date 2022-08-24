# Thinking in React and Higher-Order Functions

## Thinking in React

1. What is the single responsibility principle and how does it apply to components?
- The single responsibility function means that ever elements ideally only does one thing in the code like every function is better to only do one thing. It applies to components in the same way that each component should do one thing.

2. What does it mean to build a ‘static’ version of your application?
- Building an application with no interactivity. It only renders the data model.

3. Once you have a static application, what do you need to add?
- We should add interactivity.

4. What are the three questions you can ask to determine if something is state?
- Is it passed in from a parent via props?
- Does it remain unchanged over time? 
- Can you compute it based on any other state or props in your component?

5. How can you identify where state needs to live?
- Identify every component that renders something based on that state
- Find a common owner component
- Either the common owner or another component higher up in the hierarchy should own the state

## Higher-Order Functions
1. What is a “higher-order function”?
- They are functions that can operate on other functions like taking them as arguments or returning them.

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
- It creates a new function to compare between numbers

3. Explain how either map or reduce operates, with regards to higher-order functions.
- Map transforms the array after applying a function to the contents of the array and then return a new array with the updated values.

## Things I want to know more about
The benefits of using higher order functions and when to use them.