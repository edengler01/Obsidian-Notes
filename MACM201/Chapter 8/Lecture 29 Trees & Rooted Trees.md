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
##### <span style="color:#00b050">Theorem 7.1.6</span>
1. *G* is connected and has no cycles (*G* is a tree)
2. *G* is connected and *|V| = |E|* + 1
3. *G* has no cycle and *|V| = |E|* + 1
4. There is a unique path between every pair of vertices in *G*
<span style="font-weight:bold; color:#c00000">Proof</span>:
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


#### <span style="color:#0070c0">Rooted Trees</span>
##### <span style="color:#00b050">Definition 7.1.2: A Rooted Tree</span>
- A [[rooted tree]] *T = (V,E)* is a tree with a distinguished vertex called the [[root]]
- For every vertex *v ∈ V* of the [[level]] of *v* is the length of the path from *v* to the root.
- <span style="color:#0070c0">Note:</span> the root is the unique vertex at level 0
##### <span style="color:#ffc000">Example 7.3</span>
##### <span style="color:#00b050">Definition 7.3: Rooted Tree Terminology</span>
- The [[height]] of a rooted tree is the max level of a vertex
- Every non-root vertex *v* at level *i* is adjacent to exactly one vertex *u* at level *i-1*. We call *u the **parent*** of *v* and we say that *v* is a **child** of *u*
- A vertex of a rooted tree is **internal** if it has a child and otherwise we call it **external**. <span style="color:#0070c0">Note</span>: the root is always internal unless the tree has just one vertex
- For every vertex *v* there is a walk "up the tree" to the root obtained by moving the parent vertex at each step. If *u* is another vertex on this walk, we call *u* an **ancestor** of *v* and *v* a **descendant** of *u*
- ![[Pasted image 20231123174621.png]]
##### <span style="color:#00b050">Definition 7.4: Subtree</span>
- Let *v* be a vertex of a rooted tree *T* with level *i*. Define T^i to be the subgraph of *T* induced by *v* together with its desendants. Then T^i forms a new rooted tree with root vertex *v*. We say that T^i with root *v* is the subtree of *T* at *v*
- ![[Pasted image 20231123175405.png]]
##### <span style="color:#00b050">Definition 7.1.5: Isomorphism of rooted trees</span>
- Let T_1, T_2 be rooted tree with T_i = (V_i, E_i) for *i = 1,2*.
- T_1 and T_2 are **isomorphic as rooted trees** if there exists a bijection *f: V_1 -> V_2*: satisfying:
	1. *{f(u), f(v)} ∈ E_2 <-> {u,v}∈ E_1*
	2. For every *v∈ V_1* the level of *v* and *f(v)* is the same.
		- In particular, f sends the root of T_1 to the root of T_2
##### <span style="color:#ffc000">Example 7.4</span>
![[Pasted image 20231123175730.png]]
##### <span style="color:#00b050">Definition 7.1.6</span>
A rooted tree is m-ary if every internal node has at most *m* children. A 2-ary tree is called **binary** tree (Every vertex has 2 or less children)
##### <span style="color:#ffc000">Example 7.5</span>
- ![[Pasted image 20231123180313.png]]

##### Induction on Rooted Trees
