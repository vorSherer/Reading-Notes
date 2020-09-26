# Read 35 - Graphs

#### 2020-09-26

## RESOURCES:
### Graphs <br>
https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html <br>

---
---

## Graphs <br>
A long-ish survey of what graph structures look like, are composed of, are configured and traversed. <br>
The many variations are difficult to visualize and follow. More resources needed to get a decent handle on this data structure. <br>
### Graph terminology
Graphs are composed of __`vertices`__ linked by __`edges`__. <br>
Directly connected vertices are said to be __`adjacent`__ or "__`neighbors`__". <br>
The __`degree`__ of a vertex is the number of edges connected to that vertex. <br>
Graphs can be __`Directed`__ (Also called a __`digraph`__, with unidirectional edges. ) or __`Undirected`__ (or __`non-directed`__, with bidirectional edges). <br>

A __`complete`__ graph is when all nodes (vertices) are connected to all other nodes. <br>
A __`connected`__ graph is graph tin which all of vertices/nodes have at least one edge. <br>
A __`disconnected`__ graph is a graph where some vertices may not have edges. <br>

Graphs may also be __`cyclic`__ or __`acyclic`__: <br>
A __`cycle`__ is when a node can be traversed through and potentially end up back at itself, risking an endless loop. <br>
An __`acyclic`__ graph is a directed graph without cycles. <br>

A Graph can be represented with an __`adjacency matrix`__ or an __`adjacency list`__. <br>

A __`weighted graph`__ is a graph with __*numbers assigned to its edges*__. These numbers are called __`weights`__. <br>

### Traversing a Graph
A __`Breadth-first traversal`__ of a Graph is accomplished with a __`Queue`__. <br>
A __`Depth-first traversal`__ of a Graph is accomplished using a __`Stack`__. <br>
