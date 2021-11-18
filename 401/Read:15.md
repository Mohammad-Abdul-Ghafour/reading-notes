# Implementation: Trees

## Common Terminology:

Vocabulary | meaning
---------|---------
Node | component of the tree that has a value and reference to other nodes
Root | the first node in the tree
K | the maximum number of children of a node (In binary tree k=2)
Left/Right | used as a reference to a child of the node
Edge | the link between a parent and a child node
Leaf | A node with no children
Height | number of edges from the root node to the furthest leaf node
Traversals | the process of visiting each node in a tree only once
Depth First | traversing through the height of the tree first (using call stack)
Breadth First | iterates through the tree by going through each level of the tree node-by-node (using queue)
Binary Tree | each node have up to two children only, left and right
K-ary Trees | each node have up to K children
Binary Search Trees | a sorted tree where all the nodes on the left are smaller than the root and on the right are bigger

## Big O:
* Insert a node: O(n)
* Search for a node: O(n)

![](https://courses.engr.illinois.edu/cs225/sp2019/assets/notes/bst/bsttreetraversal.png)

## Uses of Binary trees 
* Binary Search Tree
* Binary Space Partition
* Binary Tries
* Syntax Tree
* Hash Trees
* Heaps
* Treap 
* T-Tree 
* Huffman Coding Tree (Chip Uni)
