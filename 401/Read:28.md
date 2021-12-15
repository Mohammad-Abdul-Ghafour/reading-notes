# Graphs

## Vocabulary Terms

Vocabulary | meaning
---------|---------
Graph | a non-linear data structure, consists of **nodes** connected by **edges**
Vertex (node) | a data object that could be connected to none or more nodes
Edge | the connection between two nodes
Neighbor |  nodes that are connected with an edge
Degree |  number of edges connected to a node

## Graphs uses

* used to visually illustrate relationships in the data.
* Electrical Engineering: used in designing of circuit connections
* Google Search
* Google Maps: various locations are represented as vertices or nodes and the roads are represented as edges
* GPS
* social media
  > Find more application of Graphs [Here](https://www.javatpoint.com/graph-theory-applications)

## Directed vs Undirected Graphs

![Directed vs Undirected Graphs](https://sites.google.com/a/cs.christuniversity.in/discrete-mathematics-lectures/_/rsrc/1409480658489/graphs/directed-and-undirected-graph/dir.png)

## Complete vs Connected vs Disconnected Graphs

![Complete vs Connected vs Disconnected Graphs](https://adrianmejia.com/images/connected-vs-complete-graph.jpg)


## Acyclic vs Cyclic Graphs

![Acyclic vs Cyclic Graphs](https://miro.medium.com/max/1536/1*lsf_f_JGXKA_JEPzFNMwCQ.png)

## Sparse vs Dense Graphs

![Sparse vs Dense Graphs](https://www.alberton.info/images/articles/graphs/graphs_complete_sparse.png)


## Graph Representation

### Adjacency Matrix

* It represents a graph as a 2-dimensional array.
* *nxn*  matrix indicates n vertex.
* a **one** in this matrix indicates an edge that connect between the row and column.
* a **zero** indicates the absence of the edge.

### Adjacency List

* It represents a graph as an array of linked lists.
* The index of the array represents a vertex.
* Each element in its linked list represents the other vertices that form an edge with the vertex.
