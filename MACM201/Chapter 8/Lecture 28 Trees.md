[Macm 201 - Lecture 28 - YouTube](https://www.youtube.com/watch?v=ia37wN0WbL8&t=13s&ab_channel=JamieMulholland)

### <span style="color:#c00000">Definition: Tree, Forest, Leaf</span>
Let *G = (V,E)* be a multigraph. *G* is **tree** if *G* is connected and *G* does not contain a [[cycle]]. 
*G* is a forest if G does not contain a [[cycle]]. A vertex of degree 1 is called a **leaf** or pendant vertex.
#### [[Examples of trees, forest, leaf]]
##### Note
A tree cannot have [[Loops]] or [[Parallel edges]], it is a [[simple graph]]
Every graph with all vertices of degree 2 or greater must have a [[cycle]]
	Therefore every tree with more than 2 vertices must have a leaf

#### <span style="color:#c00000">Lemma</span>
##### If *T - (V, E)* is a tree with leaf *v* then *T-v* is a tree
![[Pasted image 20231123181036.png]]
<span style="color:#0070c0">What this Lemma is saying:</span> Start with a tree -> Prune a leaf -> End up with a tree
<span style="color:#7030a0">Proof (Need to show T - v is connected & acyclic)</span>
- Since T-v is a subgraph of T, <span style="color:#ffc000">then T - v is acyclic.</span>
- To show T-v is connected, let *u,w* be 2 vertices in the graph.
- Since T is connected, let *p* be a *uw-path* 
	- Then P: 
		- ![[Pasted image 20231123181443.png]]
	- Therefore, P is a path in T-v. <span style="color:#ffc000">So T-v is connected. </span>
	- Finally, T-v is a tree
#### <span style="color:#00b050">Theorem (Unique paths)</span>
##### If *T = (V, E)* is a tree and *u, v ∈ V* are distinct, there is a unique path in T with ends *u, v*.
<span style="color:#7030a0">Proof:</span> 
- Since T is connected, there is a uv-path, say *P* <span style="font-weight:bold; color:#ffc000">(want to show that its unique)</span>
- Assume, there is another uv-path, say *Q*, such that *P =/= Q*
	- Then there must be an edge on one path that the other doesn't use.
	- Situation looks like this
		- ![[Pasted image 20231123181920.png]]
		- Looks like a cycle, but its a tree so its impossible
	- There is a ab-walk in T-e. If we remove edge e, we can walk back from a to u and take path P to v and then reach b
		- ![[Pasted image 20231123182041.png]]
	- Hence T-e is connected. So *e* is part of a cycle in T, which leads to a <span style="color:#ffc000">contradiction.</span>
		- <span style="color:#ffc000">T is a tree so it cannot have a cycle</span>
	- Therefore, path is unique.
#### <span style="color:#00b050">Theorem (main property of trees)</span>
##### 1. If *T = (V, E)* is a tree, then *|V| = |E|* + 1
##### 2. If *G = (V, E)* is a forest with K trees then *|V|* = |E| + k
<span style="color:#c00000">Proof:</span>
1. Use induction |V|
- base case: |V| = 1, |E| = 0: |V| = |E| + 1 <span style="color:#00b050">which is true</span>
- Induction Hypothesis: Assume result is true for trees with |V| = n, for some fixed n >= 2
- Inductive step: Let T be a tree with |V| = n+1
	- Let *L* be a leaf, then 
		- *T-L* is a tree with |V|-1 & |E|-1 edge.
	- By IH: |V| - 1= (|E|-1) +1
		- |V| = |E| + 1
- Finally, result holds for T with |V| = n + 1
- Result holds for all tree T.

2. Let T_1,..., T_k be the trees in the forest. Then by 1: 
	- |Vi|=|E+i| for each T_i
- Summing over  1 <= i <=k:
	- |V| = |E| + k
- Done
#### <span style="color:#c00000">Lemma</span>
##### If *G = (V,E)* satisfies *|V| = |E| + 1* then *G* must have a vertex of degree 0 or at least two of degree 1
Proof
 