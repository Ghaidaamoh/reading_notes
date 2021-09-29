# Graphs

**What is a graph?**

- In programming, a graph is a common data structure that consists of a finite set of nodes (or vertices) and edges. The edges connect the vertices to form a network. An edge can be uni-directional or bi-directional. Edges are also known as arrows in a directed graph and may contain values that show the required cost to traverse from one vertex to another.
- A vertex is similar to linked list nodes. A pair (x,y) is referred to as an edge. This communicates that the x vertex connects to the y vertex.

**Graph terminology**

![graph](Code401reading-notes/images/graph1.png)

- Degree of a vertex: The total number of edges connected to a vertex. There are two types of degrees:

  - In-Degree: The total number connected to a vertex.

  - Out-Degree: The total of outgoing edges connected to a vertex.

- Adjacency: Two vertices are said to be adjacent if there is an edge connecting them directly.

- Parallel Edges: Two undirected edges are parallel​ if they have the same end vertices. Two directed edges are parallel if they have the same origin and destination.

- Self Loop: This occurs when an edge starts and ends on the same vertex.

- Isolated vertex: A vertex with zero degree, meaning it is not an endpoint of an edge

**Types of graphs**

- undirected graph: the edges are bi-directional by default
for example, with the pair (0,1), it means there exists an edge between vertex 0 and 1 without any specific direction. You can go from vertex 0 to 1, or vice versa.

![image](Code401reading-notes/images/undirection.png)

- directed graph: the edges are unidirectional
for example, with the pair (0,1), it means there exists an edge from vertex 0 towards vertex 1, and the only way to traverse is to go from 0 to 1.

![image](Code401reading-notes/images/directional.png)

**Types of graph representations**

- Here is the two most commonly used representations: Adjacency List and Adjacency Matrix.

   - Adjacency Matrix: is a two-dimensional matrix where each cell can contain a 0 or a 1.​ The row and column headings represent the source and destination vertices respectively. If a cell contains 1, that means there’s an edge between the corresponding vertices. Edge operations are performed in constant time, as we only need to manipulate the value in the particular cell.

![image](Code401reading-notes/images/matrix.png)

- Adjacency List: an array of Linked Lists is used to store edges between two vertices. The size of the array is equal to the number of vertices. Each index in this array represents a specific vertex in the graph. If a new vertex is added to the graph, it is simply added to the array as well.

![image](Code401reading-notes/images/list.png)


**Real-world uses of graphs**

- The graph data structure plays a fundamental role in several applications:

1. GPS
2. Neural networks
3. Peer to peer networks
4. Search engine crawlers
5. Garbage collection
6. Social networking websites