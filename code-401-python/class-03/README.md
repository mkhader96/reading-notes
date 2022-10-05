# Whiteboarding + Big O


## Reading:
### The Big O Notation
-Big O notation is used in Computer Science to describe the performance or complexity of an algorithm. Big O specifically describes the worst-case scenario, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm.
- Some examples:
1. O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

`bool IsFirstElementNull(IList<String> elements)`

`{
    return elements[0] == null;
}
`

2. O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set. This is common with most loops.
`bool ContainsValue(IEnumerable<string> elements, string value)`
`{
    foreach (var element in elements)`
`{
        if (element == value)`
`{
            return true;
        }
    }`
`    return false;
}`



3. O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. 

`bool ContainsDuplicates(IList<string> elements)`
`{
    for (int outer = 0; outer < elements.Count; outer++)`
`{
        for (int inner = 0; inner < elements.Count; inner++)`
`{
            // Don't compare with self
            if (outer == inner)`
`{
                continue;
            }`
`            if (elements[outer] == elements[inner])`
`{
                return true;
            }`
`        }`
`    }`
`    return false;
}`

4. O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. The growth curve of an O(2^N) function is exponential — starting off very shallow, then rising meteorically. An example of an O(2^N) function is the recursive calculation of Fibonacci numbers:
`int Fibonacci(int number)`
`{
    if (number == 0 || number == 1)`
`{
        return number;
    }`
`    return Fibonacci(number - 1) + Fibonacci(number - 2);
}`

5. O(log N) describes an algorithm that will divide the number of items to process by half with each iteration. This is a common pattern with search algorithms.

### The Big O Notation
- The link contains a podcast between two developers talking about the Big O notation and how it is used in software development.
- It is a way of evaluating how efficient something is, and it can be used to talk about algorithms and how useful a data structure is based on the algorithm used.
- It means how much time and memory does it take.
- We can think about it as a grade for how efficient something is.
- A+ would be something called constant time, which means that no matter how much data you have, it will always take the same amount of time to run.
- They talk about multiple examples of codes and algorithms and how they are graded based on the Big O notation.
