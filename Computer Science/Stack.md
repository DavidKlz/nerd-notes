# Stack

## Definition

[Abstract data type](/Computer%20Science/Abstract%20data%20type.md) with the following operations:  

* push(Key): adds key to collection
* Key top(): returns most recently-added key
* Key pop(): removes and returns most recently-added key
* Boolean empty(): are there any elements?

## Implementation

### [Array](/Computer%20Science/Array.md)

The stack implementation can be implemented with the help of an [array](/Computer%20Science/Array.md):  

* numElements -> we create a variable to keep track of the size, push + 1 and pop - 1
* push -> appends element of the [array](/Computer%20Science/Array.md)
* top -> get the last element of the [array](/Computer%20Science/Array.md) by using our variable numElements
* pop -> take out and remove the last element
* empty -> simple check if variable numElements is greater than 0
If you take a look at the [performance of common Operations section of the array](/Computer%20Science/Array.md#performance-of-common-operations)
you will see that each operation we use has a performance of O(1),
which means the stack operations efficiently.  
The draw back of an [array](/Computer%20Science/Array.md) is its predefined size,
so if we try to push once the [array](/Computer%20Science/Array.md) is full we will get an error.

### [Linked List](/Computer%20Science/Linked%20List.md)

TO BE DONE

## Source

| Type   | Source                                                        |
| ------ | ------------------------------------------------------------- |
| Course | <https://www.coursera.org/lecture/data-structures/stacks-UdKzQ> |
