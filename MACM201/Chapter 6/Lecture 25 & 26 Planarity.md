### Definition 6.3.1: Planar Graphs
- A graph is [[planar]] if it has a drawing where the edges only intersect at vertices of G
	- Also called a planar embedding

### Definition 6.3.2: Subdivisions
- To [[subdivide]] an edge, delete edge *e* and add a new vertex *w* and two new edges *e<sub>1</sub> = {u,w}* and *e<sub>2</sub> = {w,v}* 
- If a graph is obtained from G by a sequence of subdivisions, then H is called a subdivision of G
#### Example 6.10 
- ![[Pasted image 20231129134749.png]]


### Definition 6.3.3 - Kuratowski-Wagner
- A [[multigraph]] is only planar if and only if it does not contain a subdivision of K<sub>3,3</sub> or k<sub>5</sub>
#### Note:
1. If G is planar, then every subgraph of is planar



# Faces
### Definition 6.3.4
- The embedded partitions in a graph are called faces.
	- The one unbound region that lie "outside" the graph is called the infinite face.
	- All other faces are internal faces
	- If G is connected, every face has vertices and edges on it boundary
		- They form a closed walk (a facial walk)

# Euler Formula
### Definition 6.3.2 - [[Euler's Formula]]
- If G is a connected [[multigraph]] embedded in the plane and *F* is a set of faces then
		*|V|-|E| +|F| = 2*

#### Proof
By Induction on |E| in G


##### Base Case: n = 0. 
- G is a [[singleton]] graph
- |E| = 0
- |F| = 1 (The infinite face)
- |V| = 1
- Plug into [[Euler's Formula]]
	- 1 - 0 + 1 = 2
	- <span style="color:#00b050"> 2 = 2 </span>
##### Inductive Hypothesis: Assume Euler's holds for all graphs such that |E| < n

##### Inductive Step: Assume G has a cycle
- Let *e* be an edge on the cycle. Let F<sub>I</sub> and F<sub>j</sub> be the faces separated by edge *e*.
- By removing the edge, we obtain the graph *H = G - {e}* where *|F| - 1* faces,  *|E| - 1* edges, but still have the same number of |V| and H is still connected
###### Via the inductive hypothesis
*|V| - (|E| -1) + (|F|-1) = 2*
*|V|+|E||+|F| = 2*

##### Case 2
- Assume that G has no cycle but it is connected
	- Then G has a tree (by the important lemma), A has a leaf
- By deleting a leaf from G, we obtain some graph G' = G - {v}
- G' is connected 
	- |E'| = |E| -1
	- |V'| = |V| - 1
	- |F'| = |F|
- Apply inductive to G'
	*|V'| - |E'| +|F'| = 2 (Euler formula holds)*
	