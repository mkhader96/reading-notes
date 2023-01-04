# Next- Forms and Conditional Rendering 

## Reading:
#### WHAT IS MEMOIZATION?
- There are some times when re-rendering of the component results in performance issues. To overcome this, React provides us with a performance feature known as memoization.

- Memoization is an optimization technique that allows an increase in the performance of a program by storing the results of some expensive function so that we don’t need to call that function when the same inputs are given.

#### HOW TO IMPLEMENT MEMOIZATION IN REACT
- React has the features PureComponent and memo hook which allow us to implement memoization in React.
- PureComponent allows us to perform optimization. It depends on the shouldComponentUpdate() lifecycle method but it can only be used with the class component.
- React also gives us a memo() hook to apply memoization for functional components.
- If we need a function component that gives the same result for the same props and we don’t want to re-render it, we can use memoization to skip the re-render of the component by storing and reusing the last rendered result.

#### MEMOIZATION USING PURECOMPONENT
- PureComponent is similar to Components in React except that PureComponent implements shouldComponentUpdate() with shallow prop and state comparison and Components does not.
In some cases, if our component re-renders the same result with the same given props and state which results in performance issues, then we can use PureComponent to increase performance. PureComponent’s shouldComponentUpdate() only shallowly compares the object.
- But we should make sure that props and state are simple. If they contain any complex data structures then PureComponent may produce wrong results. Also, we should make sure that all the children components of PureComponent are also PureComponent since 

- PureComponent’s shouldComponentUpdate() skips prop updates for the full component subtree.

#### WHEN TO USE MEMOIZATION
- Memoization can increase performance for some functions. But, if we use it for every component rendering, it might decrease performance since it stores results that increase memory used for the program. We should only use memoization when there is a clear benefit for doing so.

#### React Custom Hooks
- Custom React JS hooks are reusable functions that a React JS software developer can use to add special and unique functionality to the React applications. Usually, if there is a requirement to add a feature, one can install a third-party library and solve the problem. But what if there is no such library with hooks that can be used? This problem is solved by using custom React JS hooks.

#### What are the advantages of using a custom React JS hook?
- Reusability
- Readability
- Testability
