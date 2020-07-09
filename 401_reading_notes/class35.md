# Graph
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

##  common terminology in Graphs
1. Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. Edge - An edge is a connection between two nodes.
3. Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
4. Degree - The degree of a vertex is the number of edges connected to that vertex.

## Types of graphs
* Undirected: An undirected graph is a graph in which all the edges are bi-directional i.e. the edges do not point in any specific direction.
* Directed:  also called a Digraph A directed graph is a graph in which all the edges are uni-directional i.e. the edges point in a single direction.

There are many different types of graphs. **This depends on how connected the graphs are to other node/vertices.**

* Complete Graphs: A complete graph is when all nodes are connected to all other nodes.
* Connected: A connected graph is graph that has all of vertices/nodes have at least one edge.
* Disconnected: A disconnected graph is a graph where some vertices may not have edges.
* Cyclic: A graph is cyclic if the graph comprises a path that starts from a vertex and ends at the same vertex. That path is called a cycle.
* An acyclic: graph is a graph that has no cycle

## Graph Representation
We represent graphs through:
* Adjacency Matrix
An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

* Adjacency List
 the most common way to represent graphs. An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

* Weighted Graphs
A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.

## Traversals
* Breadth First
* Depth First


## Real World Uses of Graphs
Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

* GPS and Mapping
* Driving Directions
* Social Networks
* Airline Traffic
* Netflix uses graphs for suggestions of products