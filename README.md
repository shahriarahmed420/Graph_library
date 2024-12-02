# graph-library-shahriar

**graph-library-shahriar** is a Python library for performing graph traversals, including Breadth-First Search (BFS) and Depth-First Search (DFS). It also includes utility functions for adding edges to graphs and test scripts for verifying the implementation.

---

## **Features**
- Perform **Breadth-First Search (BFS)** on a graph.
- Perform **Depth-First Search (DFS)** on a graph.
- Utility functions to add edges to graphs for BFS and DFS.
- Includes test cases for BFS and DFS traversal implementations.

---

## **Installation**
You can install this library using **pip**:

```bash
pip install graph-library-shahriar


## **BFS**:

from graph_library.bfs import add_edge, bfs

# Initialize an adjacency list for the graph
V = 5  # Number of vertices
adj = [[] for _ in range(V)]

# Add edges
add_edge(adj, 0, 1)
add_edge(adj, 0, 2)
add_edge(adj, 1, 3)
add_edge(adj, 1, 4)

# Perform BFS starting from vertex 0
start_vertex = 0
result = bfs(adj, start_vertex)
print("BFS Traversal Result:", result)


## **DFS**:

from graph_library.dfs import add_edge_dfs, dfs

# Initialize an adjacency list for the graph
V = 6  # Number of vertices
adj = [[] for _ in range(V)]

# Add edges
add_edge_dfs(adj, 0, 1)
add_edge_dfs(adj, 0, 2)
add_edge_dfs(adj, 1, 3)
add_edge_dfs(adj, 1, 4)
add_edge_dfs(adj, 2, 5)

# Perform DFS starting from vertex 0
print("DFS Traversal Result: ", end="")
dfs(adj, 0)
