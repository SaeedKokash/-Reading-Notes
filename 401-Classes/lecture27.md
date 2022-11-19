# Readings: Graphs #

### What is a Graph? ###
A graph is a collection of two sets V and E where V is a finite non-empty set of vertices and E is a finite non-empty set of edges.

- Vertices are nothing but the nodes in the graph.
- Two adjacent vertices are joined by edges.
- Any graph is denoted as G = {V, E}.

![graph](https://media.geeksforgeeks.org/wp-content/cdn-uploads/undirectedgraph.png)

``` G = {{V1, V2, V3, V4, V5, V6}, {E1, E2, E3, E4, E5, E6, E7}}  ```

### Tree ###
A tree is a finite set of one or more nodes such that –

- There is a specially designated node called root.
- The remaining nodes are partitioned into n>=0 disjoint sets T1, T2, T3, …, Tn 
- where T1, T2, T3, …, Tn are called the subtrees of the root.

The concept of a tree is represented by following Fig.

![tree](https://media.geeksforgeeks.org/wp-content/cdn-uploads/binary-tree-to-DLL.png)


### Graph vs Tree ###
| Comparison | Graph | Tree |
| Definition | Graph is a non-linear data structure. 	 | Tree is a non-linear data structure. |
| Structure | 	It is a collection of vertices/nodes and edges. | It is a collection of nodes and edges. |
| Edges | Each node can have any number of edges.	 | If there is n nodes then there would be n-1 number of edges |
| Types of Edges | They can be directed or undirected	 | They are always directed There is no unique node called root in graph.	|
| Root node	 | There is no unique node called root in graph.	 | There is a unique node called root(parent) node in trees. |
| Loop Formation	 | A cycle can be formed.	 | There will not be any cycle. |
| Traversal	 | For graph traversal, we use Breadth-First Search (BFS), and Depth-First Search (DFS).	 | We traverse a tree using in-order, pre-order, or post-order traversal methods. |
| Applications	 | For finding shortest path in networking graph is used.	 | For game trees, decision trees, the tree is used. |

### Types of Graphs ###

1. Finite Graphs
2. Infinite Graph
3. Trivial Graph
4. Simple Graph
5. Multi Graph
6. Null Graph
7. Complete Graph
8. Pseudo Graph
9. Regular Graph
10. Bipartite Graph
11. Labeled Graph
12. Digraph Graph
13. Subgraph
14. Connected or Disconnected Graph
15. Cyclic Graph
16. Types of Subgraphs

### *[Source01](https://www.geeksforgeeks.org/difference-between-graph-and-tree/)*  *[Source02](https://www.geeksforgeeks.org/graph-types-and-applications/?tab=article)*  *[Source03](https://www.geeksforgeeks.org/basic-properties-of-a-graph/)* 
