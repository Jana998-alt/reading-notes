# Graphs

Graphs are a datastructure that have nodes and verticies, where nodes are connected to each other through the verticies. they are used for transportation systems implementation. 

list of terminology: 
Vertex --->	Every individual data element is called a vertex or a node. In the above image, A, B, C, D & E are the vertices.
Edge --->	It is a connecting link between two nodes or vertices. Each edge has two ends and is represented as (startingVertex, endingVertex).
Undirected Edge	---> It is a bidirectional edge.
Directed Edge	---> It is a unidirectional edge.
Weighted Edge --->	An edge with value (cost) on it.
Degree---> The total number of edges connected to a vertex in a graph.
Indegree	---> The total number of incoming edges connected to a vertex.
Outdegree --->	The total number of outgoing edges connected to a vertex.
Self-loop --->	An edge is called a self-loop if its two endpoints coincide with each other.

## methods of implementing the Graphs

- Adjacency Matrix which is an array of zeros and ones, where the one represents a connection between nodes.
- Adjacency List is an array of linked lists. where the linked list represents the nodes connected to the first head.

Graphs can be:
- connected vs disconnected ---> all nodes are connected to another node vs some nodes do not have connections.
- complete ---> all nodes are connected to each other
