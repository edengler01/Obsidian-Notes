What is an [[Articulation Point]]?
- A vertex where if you remove it from the graph G, the graph becomes disconnected



### Lemma 7.3.1
- A vertex is an [[Articulation Point]] iff there are distinct x=/=y=/= v and every path between x & y includes v
	- Example: Picture ![[Pasted image 20231128025200.png]]


### Definition 7.3.2: Biconnected
- If the graph is connected, then it has no [[Articulation Point]]

### Definition 7.3.3 Biconnected Component
- A maximal subgraph of G 


#### 1st Algorithm for finding AP
- Go through every vertex and check if its connected
	- Checking each vertex takes O(n) time
	- Checking if that vertex disconnects takes O(n) time
	- Therefore it takes O(n^2) to complete this algorithm

#### 2nd Algorithm for finding AP
1. Construct a [[Depth First Search]] spanning tree & number of edges in T in order visited rooted at d, assume alphabetical ordering
2. Look at where the [[Articulation Point]]s are
	- a leaf is not an AP
	- the root is an AP
	- if a child in the graph has no [[back edges]]
	- Then renumber all the edges on the walk to the edge traveresed

##### What are the APs?
- The vertices that are incident with edges with different labels

##### What are the biconnected components?
- The maximal subgrahs of T + {[[back edges]]} with equal edge labels