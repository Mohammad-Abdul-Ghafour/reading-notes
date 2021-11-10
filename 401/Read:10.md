# Stacks and Queues
What is a Stack ?....

A **`Stack`** is a data structure that consists of **`Nodes`**.Each **`Node`** references the next Node in the stack, but does not reference its previous.

Common terminology for a stack is:

terminology | meaning
---------|---------|
Push | means adding a node to the stack
Pop | means removing a node from the stack
Top | refers to the top of the stack
Peek | means to view the value of the top node in Stack and the front node in a queue
IsEmpty | checks if the stack or the queue is empty

vocabularies | meaning
---------|---------|
Stacks | type of structuring data with nodes and a reference to next node.
Dequeue | nodes that are removed from the queue
Enqueue | nodes that are added to the queue
Front/Rear | first/last node in the queue


![Queues](https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Data_Queue.svg/1200px-Data_Queue.svg.png)


## FILO vs. LIFO:
* **`Stack`** : 
    1. **`LIFO`** : Last In First Out.
    2. **`FILO`** : First In Last Out.
2. **`Queue`** :
    1. **`FIFO`** : Fist In First Out.
    2. **`LILO`** : Last In Last Out.

![](https://carminati.altervista.org/PROJECTS/C++/FIFO%20and%20LIFO/IMG/FIFO-LIFO.png)


## Example of a Stack Implementation Using Queue Module :

1. **`CODE`** :

```python
# Python program to
# demonstrate stack implementation
# using queue module
 
from queue import LifoQueue
 
# Initializing a stack
stack = LifoQueue(maxsize=3)
 
# qsize() show the number of elements
# in the stack
print(stack.qsize())
 
# put() function to push
# element in the stack
stack.put('a')
stack.put('b')
stack.put('c')
 
print("Full: ", stack.full())
print("Size: ", stack.qsize())
 
# get() function to pop
# element from stack in
# LIFO order
print('\nElements popped from the stack')
print(stack.get())
print(stack.get())
print(stack.get())
 
print("\nEmpty: ", stack.empty())
```

2. **`OUTPUT`** :

```
0
Full:  True
Size:  3

Elements popped from the stack
c
b
a

Empty:  True
```