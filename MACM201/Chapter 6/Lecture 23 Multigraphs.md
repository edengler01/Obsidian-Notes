### Reminder of graph terminology
[[Vertices]]
[[Edge]]
[[Edge set]]
**[[Loops]]**

[[Multiset]]
[[Size/Cardinality]]

## A more general kind of graph

<span style="color:#c00000">Definition 6.1.1 - A Multigraph</span>
- When *G = (V,E)* is a set of *V* of [[Vertices]] and a [[Multiset]] *E* of edges where each edge is in *V x V*
<span style="color:#0070c0">Note:</span> An edge *e* that is [[incident]] to one vertex is called a loop
- We think of *e* as having two "ends" that are both at the vertex.
- [[Parallel edges]] are where two distinct edges are both incident to them selves


<span style="color:#ffc000">Example 6.1</span>![[Pasted image 20231123125559.png]]
<span style="color:#0070c0">Note</span>: A [[simple graph]] are multigraphs with no [[Loops]] and no [[Parallel edges]]
End of [[Definition 6.1.1 - A Multigraph]]


## Walks, Trails and Circuits
<span style="color:#c00000">Definition 6.1.2 -  Walks in Multigraphs</span>
- Let *x* and *y* be two [[Vertices]] in a multigraph ([[Definition 6.1.1 - A Multigraph]]).
- A [[walk]] in *G* is a finite alternating sequence
-  The **length of the walk** *n* is the number of edges
- A **closed walk** is a walk that starts and ends at the same verted
	- Otherwise, it is consider a open walk
<span style="color:#0070c0">Note</span>: [[Vertices]] and edges do not need to be unique
- A walk of length 0 involves on vertex and no edges. It is called a trivial walk.

<span style="color:#ffc000">Example 6.2</span>
![[Pasted image 20231123130414.png]]

<span style="color:#c00000">Definition 6.1.3- Trails and Circuits</span>
- A [[path]] from *x to y* is a walk in G that has no repeated vertices
- A trail from *x to y* is an open walk in *G* where each edge appears no more than its multiplicity
- A circuit from  *x to x* is a closed walk in *G* in which each edge appears no more than its multiplicity ([[vertices]] can be repeated)
- Example: ![[Pasted image 20231123130656.png]]

<span style="font-weight:bold; font-weight:bold; font-weight:bold; font-weight:bold; font-weight:bold; color:#00b050">Theorem 6.1.1 Trails and Paths</span>

## Degree of a vertex
Example 6.4
<span style="color:#00b050">Theorem 6.1.2</span>

## Connectivity
Example 6.5

## Direct Graphs
<span style="color:#00b050">Definition 6.1.6 Directed Graphs</span>