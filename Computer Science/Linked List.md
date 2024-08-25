# Linked Lists

A linked list works with pointers, it has a head (pointer) and can have a tail (pointer) which point to the first and last node.  

## Singly

A node of a singly linked list contains an element and a pointer to the next node.
If the pointer of a node is null we have reached the end of the linked list.

## Doubly

In a doubly linked list each node contains the element and two pointers, one pointer to next and another pointer to the previous node.
If one of the pointers is null, we have either reached the first or last node.

## Operations

* pushFront(Key) -> add to front
* Key topFront() -> return front > note
* popFront() -> remove front node
* pushBack(Key) -> add to back
* Key topBack() -> return back node
* popBack() -> remove back node
* Boolean find(Key) -> is key in list?
* erase(Key) -> remove key from list
* Boolean empty() -> empty list?
* addBefore(Node, Key) -> adds key before node
* addAfter(Node, Key) -> adds key after node

## Performance of Operations

### Singly

| Operations | Head-Pointer | Head- & Tail-Pointer |
| ---------- | ------------ | -------------------- |
| pushFront  | O(1)         | O(1)                 |
| topFront   | O(1)         | O(1)                 |
| popFront   | O(1)         | O(1)                 |
| pushBack   | O(n)         | O(1)                 |
| topBack    | O(n)         | O(1)                 |
| popBack    | O(n)         | O(n)                 |
| find       | O(n)         | O(n)                 |
| erase      | O(n)         | O(n)                 |
| addBefore  | O(n)         | O(n)                 |
| addAfter   | O(1)         | O(1)                 |

### Doubly

| Operations | Head-Pointer | Head- & Tail-Pointer |
| ---------- | ------------ | -------------------- |
| pushFront  | O(1)         | O(1)                 |
| topFront   | O(1)         | O(1)                 |
| popFront   | O(1)         | O(1)                 |
| pushBack   | O(n)         | O(1)                 |
| topBack    | O(n)         | O(1)                 |
| popBack    | O(n)         | O(1)                 |
| find       | O(n)         | O(n)                 |
| erase      | O(n)         | O(n)                 |
| addBefore  | O(1)         | O(1)                 |
| addAfter   | O(1)         | O(1)                 |

## Source

| Type    | Source |
| ------- | ------ |
| Course: | [Singly](https://www.coursera.org/lecture/data-structures/singly-linked-lists-kHhgK) |
| Course: | [Doubly](https://www.coursera.org/lecture/data-structures/doubly-linked-lists-jpGKD) |
