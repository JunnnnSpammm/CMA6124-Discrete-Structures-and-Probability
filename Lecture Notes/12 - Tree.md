# Tree

## What you will learn in this lecture:
- What is a tree?
- Some definitions and terms
- Binary tree
- Tree traversal
- Spanning tree
- Tree searching

## Tree
- A tree is a connected graph with no circuit.
- In computer science, trees are often used to describe a method for traversing a search space.
- **Theorem:** A tree with $n \ge 1$ vertices has (n – 1) edges.
- **Corollary:** Adding any edge to a tree creates a cycle (or circuit).

## Definitions and terms
- A **rooted tree** is a tree in which one vertex has been designated as the root and every edge is directed away from the root.
- If v is a vertex in a tree other than the root, the parent of v is the unique vertex u such that there is a directed edge from u to v.
- When u is the parent of v, v is called a child of u.
- Vertices with the same parent are called siblings.
- The ancestors of a vertex are the vertices in the path from the root to this vertex.
- The descendants of a vertex v are those vertices that have v as an ancestor.
- A vertex of a tree is called a leaf if it has no children.
- If x is a vertex in a tree, the sub-tree with x as its root is the sub-graph of the tree consisting of x and its descendants and all edges incident to these descendants
- The **height** of a tree is the maximum of the lengths of simple paths from the root to the leaves.

## Binary tree
- A binary tree is a tree, where every node has at most two children.
- One drawn to the left, called the left child, another drawn to the right, called the right child.
- Every node in a binary tree is the root of at most two sub-trees, namely, its left sub-tree, and the right sub-tree.

## Tree traversal
- Visiting a node in a tree generally means retrieving the data item contained in the node, and sending it to some processes such as, printing.
- There are three ways in which one could traverse all the nodes in a tree.
  * Pre-order traversal
  * In-order traversal
  * Post-order traversal

## Pre-order traversal
- Visit the current node.
- Traverse the left sub-tree of the current node.
- Traverse the right sub-tree of the current node.

## In-order traversal
- Traverse the left sub-tree of the current node.
- Visit the current node.
- Traverse the right sub-tree of the current node.

## Post-order traversal
- Traverse the left sub-tree of the current node.
- Traverse the right sub-tree of the current node.
- Visit the current node.

## Subgraph
Let G be a graph with vertex set V and edge set E, a graph H is said to be a subgraph of G $\leftrightarrow$ every vertex in H is also a vertex in G, every edge in H is also an edge in G and every edge in H has the same endpoints as it has in G.

## Spanning tree
A spanning tree of a graph G = (V, E), is a subgraph of G that is a tree containing every vertex of G.

**Theorem:**
> Any connected graph G contains a spanning tree.

- We can proof this theorem by induction on the number of edges (for info)
- Inductive Base: If $G_1$ has one edge, then the edge with its endpoints is a spanning tree of $G_1$
- Inductive Hypothesis: Assume that any connected graph with number of edges $\le$ k, $G_k$ , has a spanning tree.
- Inductive Step: We need to prove that we can find a spanning tree for any connected graph with k+1 edges, $G_{k+1}$.
  * If $G_{k+1}$ has no circuit, then $G_{k+1}$ is a spanning tree itself.
  * If $G_{k+1}$ has a circuit C, we can remove any edge e from C and $G_{k+1}$ - {e} is still connected. Since $G_{k+1}$ – {e} has one edge less, it contains a spanning tree T by induction, where T is also a spanning tree for $G_{k+1}$.

## Finding a spanning tree from a graph
- **Depth-first search (DFS)** and **breadth-first search (BFS)** can be used to find a spanning tree of a graph or to search a tree for a particular data.
- For DFS we start by selecting any vertex $V_0$, and add it to a stack S. It is a Last In First Out (LIFO) process. A helpful analogy is to think of a stack of books; you can remove only the top book, also you can add a new book on the top.
- For BFS we start by selecting any vertex V0, and add it to a queue Q. It is a First In First Out (FIFO) process. An excellent example of a queue is a line of customer in front of a bank counter. New additions to a line are made to the back of the queue, while removal (or serving a queue) happens at the front of a queue.
- BFS and DFS are widely used in games design, such as in tic-tac-toe and chess games.

## Depth-first search (DFS)
- The basic idea of depth-first search is to go as deeply as possible into a path before reaching out to other vertices.
- To find a spanning tree by DFS of a graph, start by selecting any vertex $_V0$, and add it to a stack S.
- The stack is processed as follows:
  * If vertex V is at the top of the stack S, we find its neighbours (that haven't been discovered before) and add them to the stack.
  * A vertex at the top of the stack is removed from the stack if all of its neighbours have been discovered and added to the stack.

## Breadth-first search (BFS)
- The basic idea of breadth-first search is to reach out to as many vertices as possible before penetrating deep into the next level.
- To find a spanning tree by BFS of a graph, start by selecting any vertex $V_0$, and add it to a queue Q.
- The queue is processed as follows:
  * If vertex V is at the front of the queue Q, we find its neighbours (that haven't been discovered before) and add them to the queue.
  * A vertex at the front of the queue is removed from the queue if all of its neighbours have been discovered and added to the queue.

## Summary
Materials covered in this lecture:
- Introduction to tree and its related terms, binary tree, spanning tree.
- Tree traversal.
- Apply BFS and DFS to find a spanning tree from a graph.
