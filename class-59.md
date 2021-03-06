# Graphs

A graph is a pictorial representation of a set of objects where some pairs of objects are connected by links. The interconnected objects are represented by points termed as `vertices`, and the links that connect the vertices are called `edges`.

![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/undirectedgraph.png)

a graph is a pair of sets (V, E), where V is the set of vertices and E is the set of edges, connecting the pairs of vertices. 

### some important terms:

- Vertex − Each node of the graph is represented as a vertex. In the following example, the labeled circle represents vertices. Thus, A to G are vertices. We can represent them using an array as shown in the following image. Here A can be identified by index 0. B can be identified using index 1 and so on.

- Edge − Edge represents a path between two vertices or a line between two vertices. In the following example, the lines from A to B, B to C, and so on represents edges. We can use a two-dimensional array to represent an array as shown in the following image. Here AB can be represented as 1 at row 0, column 1, BC as 1 at row 1, column 2 and so on, keeping other combinations as 0.

- Adjacency − Two node or vertices are adjacent if they are connected to each other through an edge. In the following example, B is adjacent to A, C is adjacent to B, and so on.

- Path − Path represents a sequence of edges between the two vertices. In the following example, ABCD represents a path from A to D.

![](https://www.tutorialspoint.com/data_structures_algorithms/images/graph.jpg)

### Basic Operations

- Add Vertex − Adds a vertex to the graph.

- Add Edge − Adds an edge between the two vertices of the graph.

- Display Vertex − Displays a vertex of the graph.

### Traversal

Breadth and depth example: 

![](https://open4tech.com/wp-content/uploads/2019/01/BFS-DFS.png)