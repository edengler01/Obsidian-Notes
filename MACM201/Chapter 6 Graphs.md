## Lecture 23 (Grimaldi 11.1)
### Graph Terminology
[[Vertices]]
[[Edge]]
[[Edge set]]
[[Loop]]
[[Multiset]]
[[Cardinality]]


#### Definition 6.1.1
A [[multigraph]] *G=(V,E)* is a set of *V* of [[Vertices]] and a [[Multiset]] E of edges where each edge is in *V x V*
An [[Edge]] *e* that is [[incident]] with just one vertex, say *v* is called a loop
	- We think of *e* as having two "ends" that are both at vertex *v*
	- If *f,f'∈E* are distinct edges that are both incident with the same vertices, we call them parallel
##### Example 6.1 
- Insert Drawing here



#### Walks, Trails and Circuits
#### Definition 6.1.2 - Walks in multigraphs
A walk in the graph is a finite alternating sequence
	xe1x1e2x2e3.....en-1xn-1eny
The length of the walk is *n* (the number of edges)
A walk from x to y is called a close walk if n >= 1 and x = y
	Other wise it is called an open walk
		DRAWING HERE
	Keep in mind, vertices and edges in walks need not be distinct
		DRAWING HERE
#### Definition 6.1.3- Trails and Circuits
DRAWING HERE

#### Theorem 6.1.1 - Trails & Paths
##### Proof

#### Definition 6.1.4 - Degree of a Vertex
##### Example 6.4
### Theorem 6.1.2
##### Proof


## Lecture 24 (Grimaldi 11.3)

## Lecture 25 & 26 (Grimaldi 11.4)
### Planarity
#### Definition 6.3.1
A graph G is planar if G has a drawing (in the plane) so that the edges intersect only at the vertices of G. Such a drawing is called an planar embedding of G.
##### Example 6.9
DRAWING HERE
##### Two nonplanar graphs
###### Observation
- The graph k3,3 is not planar
###### Proof Sketch
DRAWING GOES HERE
###### Observation
- The graph k5 is not planar
###### Proof Sketch
DRAWING GOES HERE

##### Definition 6.3.2 - Subdivision
##### Example 6.10
###### Observation

#### Example 6.11
- DRAWING GOES HERE
## Lecture 27 (Grimaldi 11.5)
### Hamiltonian Paths & Cycles
