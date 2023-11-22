# <span style="color:#7030a0">Lecture 28</span>
### <span style="color:#c00000">Definition: Tree, Forest, Leaf</span>
Let *G = (V,E)* be a multigraph. *G* is **tree** if *G* is connected and *G* does not contain a [[cycle]]. 
*G* is a forest if G does not contain a [[cycle]]. A vertex of degree 1 is called a **leaf** or pendant vertex.
#### [[Examples of trees, forest, leaf]]
##### Note
A tree cannot have [[loops]] or [[parallel edges]], it is a [[simple graph]]
Every graph with all vertices of degree 2 or greater must have a [[cycle]]
	Therefore every tree with more than 2 vertices must have a leaf

#### <span style="color:#c00000">Lemma</span>
##### If *T - (V, E)* is a tree with leaf *v* then *T-v* is a tree
Proof


#### <span style="color:#00b050">Theorem (Unique paths)</span>
##### If *T = (V, E)* is a tree and *u, v ∈ V* are distinct, there is a unique path in T with ends *u, v*.
Proof:
#### <span style="color:#00b050">Theorem (main property of trees)</span>
##### 1. If *T = (V, E)* is a tree, then *|V| = |E|* + 1
##### 2. If *G = (V, E)* is a forest with K trees then *|V|* = |E| + k
Proof:
#### <span style="color:#c00000">Lemma</span>
##### If *G = (V,E)* satisfies *|V| = |E| + 1* then *G* must have a vertex of degree 0 or at least two of degree 1
Proof
 
# <span style="color:#7030a0">Lecture 29</span>
#### Review

##### <span style="color:#00b050">Definition 7.1.1</span>
A multigraph *G* is a tree if G is connected and does not contain a cycle

##### <span style="color:#00b050">Theorem 7.1.3 & 7.1.2 - Main Properties of a Tree</span>
If *T = (V, E)* is a tree, then:
	- *|V| = |E|*  + 1
	- there is a unique path in T between every pair of Vertices *T*
##### <span style="color:#ffc000">Example 7.2</span>
![[Pasted image 20231122142102.png]]
<span style="color:#ffc000">Observation</span>: Removing an edge = disconnecting the graph. Adding an edge to a tree = giving it a [[cycle]]

#### <span style="color:#00b050">Characterization of Trees</span>
1. *G* is connected and has no cycles (*G* is a tree)
2. *G* is connected and *|V| = |E|* + 1
3. *G* has no cycle and *|V| = |E|* + 1
4. There is a unique path between every pair of vertices in *G*

<span style="color:#c00000">Proof</span>:
- <span style="color:#ffc000">1 -> 2</span>: Given the graph G is connected and has no [[cycle]] (is a [[tree]]), then G is connected & *|V| = |E|* + 1
- <span style="color:#ffc000">2 -> 3</span>: Given the graph G is connected and *|V| = |E|* + 1
	- To Prove: G has no cycle and *|V| = |E|* + 1
	- <span style="color:#c00000">Proof: Induction on |V| = n</span>
		- Base Case: *n = 1*
		- |V| = 1, |E| = 0
			- |V| = |E|+ 1
			- G has no cycle
	- <span style="color:#c00000">Inductive Hypothesis: Assume 2 -> 3 holds for G with |V| less than n </span>
		- If |V| = |E| + 1, G has a vertex of degree 0 or greater than or equal to 2
		- The size of |V| is greater than 1 and G is connected
			- G has a loop vertex
		- Recall that G - v is connected since G is connected & satisfies |V| = |E| + 1
	-<span style="color:#0070c0"> Therefore, in G-v, |V|-1 = (|E|-1) + 1 since G-v has more than 1 vertices by the Inductive Hypothesis, G-v has no cycle.
	- This implies that G has no cycle because v is a leaf</span>
- <span style="color:#ffc000">3 - > 1</span>: G has no cycle and |V| = |E| + 1
##### <span style="color:#00b050">Theorem 7.1.6</span>

###### Proof

#### <span style="color:#0070c0">Rooted Trees</span>
##### <span style="color:#ffc000">Example 7.3</span>
##### <span style="color:#00b050">Definition 7.3: Rooted Tree Terminology</span>
##### <span style="color:#00b050">Definition 7.4: Subtree</span>
##### <span style="color:#00b050">Definition 7.1.5: Isomorphism of rooted trees</span>
##### <span style="color:#ffc000">Example 7.4</span>
##### <span style="color:#00b050">Definition 7.1.6</span>
##### <span style="color:#ffc000">Example 7.5</span>

##### Induction on Rooted Trees

# <span style="color:#7030a0">Lecture 30</span>