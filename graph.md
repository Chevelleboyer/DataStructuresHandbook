# Graph

A graph is a non-linear data structure. All trees and linked lists are instances of graphs, but not all graphs are trees or linked lists. A graph has a key and a value. Graphs consist of vertices and edges. Edges are the connections between vertices. They can be directed (like a one way street) or not, meaning you can follow the edges in which way. Edges also can have a weight or a cost of going from one vertex to another.

# In Memory

In memory, a graph looks like this:

![Image of Array in Memory](images/array_memory.png)

\[This is what a graph looks like in memory when implemented using an adjacency list. In this implementation vertices are stored as objects and each vertex stores a list of adjacent vertices.\]

# Operations

A graph supports the following operations:

* **addVertex**: If implemented as an adjacency list the complexity of adding a new vertex is O(1). This is because we are just adding a new instance of a vertex.
* **addEdge**: This operation will add a new edge connecting vertices. If implemented as an adjacency list the complexity is O(1) because we are just adding another adjacent vertex into the list of this vertex.
* **removeVertex**: The complexity of removing a vertex is O(E) where E is the number of edges. This is because we also have to remove each of the edges conencted the the vertex we want to remove.
* **removeEdge**: Likewise, the complexity of removing an edge is O(V) because we have to find all of the vertices that this edge connected.

A graph is used to represent a network, so it is useful in many problems. Like representing phone networks. Another example would be friends on facebook. Each vertex would be a person with their information, and the edges connect friends and friends of friends.

# Example

```
myGraph = Graph() 

myGraph.addVertex(1) #adds a vertex to myGraph with a key of 1
myGraph.addVertex(7) #adds a vertex to myGraph with a key of 7
myGraph.addEdge(1, 7, 22) #adds an edge from key 1 to key 7 with a weight of 22
```

(c) 2018 Chevelle Boyer. All rights reserved.