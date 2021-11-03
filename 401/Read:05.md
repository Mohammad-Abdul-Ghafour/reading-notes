# Linked Lists

* A way to organize the data
* The node have the data of the link.
* For traversal : can't use *`forEach`* or *`for`* because *`next`* property does that, use 'while'.
```
A node only knows about what data it contains, and who its neighbor is.
```

## Array vs. Linked Lists :

Array  | Linked Lists
---------|---------
linear data structure | linear data structure
saved in one block in the memory | saved throughout the memory
static data structure |  dynamic data structure
preferable for searching | preferable for inserting and deleting

## Vocabulary Terms :

Term | meaning
---------|---------
Linked List | is a A  linear data structure (list) of linked `nodes`, each node refer to the next one.
Singly| type of linked lists where each node have one reference to the next node in the list.
Doubly |  type of linked lists where each node have two reference to the next node and previous node in the list.
Circular | type of linked lists where the last node refers to the first node.
head | a reference to the first node in the list.
current | a reference to the current node in the list.
next | a reference to the next node in the list.
previous | a reference to the previous node in the list.
null | indicates the end of the list.

![Vocabulary Terms](https://cdn.programiz.com/sites/tutorial2program/files/linked-list-concept_0.png)

## Linked Lists and Big O :

Linked Lists  | Big O
---------|---------
insert a new node at the beginning | O(1)
insert a new node at the end or the middle | O(n) because it has toloop through all list
Searching for a value | O(n) for time, O(1) for space

