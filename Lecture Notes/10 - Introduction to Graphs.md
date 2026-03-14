# Introduction to Graphs

## What you will learn in this lecture:
- Structure of graph
- Some terminologies and definitions
- Some special graphs
- Subgraphs
- Adjacency matrix
- The concept of a degree in a graph
- The Handshaking Lemma

## Graph
- A graph is a very simple (and thus very general) data structure
- Definition: A graph G = (V, E) consists of a set V of vertices (or nodes), together with a set E of edges which join two vertices.
- For the above graph we have
  * Vertex set, V = {u, v, w, z}
  * Edge set, E = {uw, vw, zw, vv}
  * Thus G = ({u, v, w, z}, {uw, vw, zw, vv})

Note 1: uw has the same meaning as wu
Note 2: If the edges are labelled, then the edges is written according to the label instead of the vertices endpoints.

## Why are graphs important?
**Where are graph used?**

Networks are graphs:
- Computer networks (computing grids, the internet)
- Telephone networks
- Social networks (who's friends with whom on Facebook), family trees, etceteras.
- Transportation, shipping routes, roads, etceteras.

Usage in Computer science:
- Dependency trees for software, pathfinding, optimisation, etceteras.

## Some terminologies and definitions
Let G = (V, E)
- An edge that connects a vertex back to itself is called a loop.
- Two distinct edges with same set of vertices endpoints are said to be parallel.
- Let v and w be vertices of G. If v and w are joined by an edge e, then v and w are said to be **adjacent** and e is said to be **incident** on v and w.
- Two edges incident on the same endpoint are called **adjacent**.
- A vertex that is an endpoint to a loop is called adjacent to itself.
- A vertex with no edges are incident is called isolated.
- A **simple graph** is a graph that does not have any loops or parallel edges
- A graph is called **connected** if there is a path from any vertex to any other vertex, otherwise the graph is **disconnected**.

## Directed graph
- In a graph, an edge is joining 2 vertices but does not provide any information on how the vertices are connected (no direction). Therefore, there is a need for having directed graphs.
- A directed graph (digraph) G = (V, E) consists of a set of vertices (or nodes) and a set of edges (or arcs) such that each edge $e \in E$ is associated with an ordered pair of vertices.

V = {a, b, c, d}, E = {ab, ac, ad, bd, cd}

Note: Here we cannot write ab as ba because this is a digraph

## Subgraph
- Let G be a graph with vertex set V and edge set E, a graph H is said to be a subgraph of G $\leftrightarrow$ every vertex in H is also a vertex in G, every
edge in H is also an edge in G and every edge in H has the same
endpoints as it has in G.

## The concept of a degree in a graph
- Let v be a vertex of a graph G, the degree of v, deg(v), equals to the number of edges that are incident on v.
- An edge that is a loop will be counted twice towards the degree.
- The total degree of G is the sum of the degree of all the vertices of G.
- **The Handshaking Lemma says that:** The sum of the degrees of all vertices of G equals twice the number of edges of G.

## Adjacency matrix
Let G be a graph with n vertices labeled 1,2,3,…,n. The adjacency matrix $A_G$ is the n x n matrix in which the entry in row i and column j is the number of edges joining the vertices i and j.

## Summary
Materials covered in this lecture?
- The structure of graph
- Some important terminologies related to graph
- Some special graphs
- The concept of degree
- The handshaking lemma
- The adjacency matrix
