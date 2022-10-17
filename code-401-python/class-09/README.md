# LinkedList

## Reading:

### What is the data structure?
#### Data Structure:
- A data structure is a specialized format for organizing, processing, retrieving and storing data. There are several basic and advanced types of data structures, all designed to arrange data to suit a specific purpose. Data structures make it easy for users to access and work with the data they need in appropriate ways. Most importantly, data structures frame the organization of information so that machines and humans can better understand it.

#### Uses of Data Structures:
- Storing data
- Managing resources and services
- Data exchange
- Ordering and sorting
- Indexing
- Searching
- Scalability

#### Characteristics of Data Structures:
- Data structures are often classified by their characteristics. The following three characteristics are examples:
1. Linear or non-linear
2. Homogeneous or heterogeneous
3. Static or dynamic

#### Data Types:
- The typical base data types include the following:
1. Integer
2. Floating-point numbers
3. Characters
4. Strings
5. Boolean
6. Fixed-point numbers
7. Pointers

#### Types of Data Structures:
- The most common types of data structures include the following:
1. Array: An array stores a collection of items at adjoining memory locations. Items that are the same type are stored together so the position of each element can be calculated or retrieved easily by an index. Arrays can be fixed or flexible in length.
2. Stack: A stack stores a collection of items in the linear order that operations are applied. This order could be last in, first out (LIFO) or first in, first out (FIFO).
3. Queue: A queue stores a collection of items like a stack; however, the operation order can only be first in, first out.
4. Linked list: A linked list stores a collection of items in a linear order. Each element, or node, in a linked list contains a data item, as well as a reference, or link, to the next item in the list.
5. Tree: A tree stores a collection of items in an abstract, hierarchical way. Each node is associated with a key value, with parent nodes linked to child nodes -- or subnodes. There is one root node that is the ancestor of all the nodes in the tree.
6. Heap: A heap is a tree-based structure in which each parent node's associated key value is greater than or equal to the key values of any of its children's key values.
7. Graph: A graph stores a collection of items in a nonlinear fashion. Graphs are made up of a finite set of nodes, also known as vertices, and lines that connect them, also known as edges. These are useful for representing real-world systems such as computer networks.
8. Trie: A trie, also known as a keyword tree, is a data structure that stores strings as data items that can be organized in a visual graph.
9. Hash table: A hash table -- also known as a hash map -- stores a collection of items in an associative array that plots keys to values. A hash table uses a hash function to convert an index into an array of buckets that contain the desired data item.

### What is a linked list?
#### Linked List:
- Linked List is a sequence of links which contains items. Each link contains a connection to another link. Linked list is the second most-used data structure after array. 
- Following are the important terms to understand the concept of Linked List:
1. Link − Each link of a linked list can store a data called an element.
2. Next − Each link of a linked list contains a link to the next link called Next.
3. LinkedList − A Linked List contains the connection link to the first link called First.

#### Types of Linked List:
1. Simple Linked List − Item navigation is forward only.
2. Doubly Linked List − Items can be navigated forward and backward.
3. Circular Linked List − Last item contains link of the first element as next and the first element has a link to the last element as previous.

#### Basic Operations:
- Following are the basic operations supported by a list.
1. Insertion − Adds an element at the beginning of the list.
2. Deletion − Deletes an element at the beginning of the list.
3. Display − Displays the complete list.
4. Search − Searches an element using the given key.
5. Delete − Deletes an element using the given key.

### Implementing a Linked List
#### Advantages of Linked List:
1. Because of the chain-like system of linked lists, you can add and remove elements quickly. This also doesn't require reorganizing the data structure unlike arrays or lists. Linear data structures are often easier to implement using linked lists.
2. Linked lists also don't require a fixed size or initial size due to their chainlike structure.
#### Disadvantages of Linked List:
1. More memory is required when compared to an array. This is because you need a pointer (which takes up its own memory) to point you to the next element.
2. Search operations on a linked list are very slow. Unlike an array, you don't have the option of random access.