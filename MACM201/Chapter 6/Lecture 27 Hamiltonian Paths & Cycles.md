Recall [[Hamiltonian vs Eulerian]]

### Definition 6.4.2 Necessary and Sufficient Conditions
1. C is necessary for P if every graph satisfying P also satisfies C (P -> C)
2. C is sufficient for P if every graph satisfying C also satisfies P (C -> P)
3. If C is both for P, then a graph G satisfies P iff G satisfies C. We say C characterize P.
#### Example 6.18
1. It is necessary for G to be connected to have a HP
	- HP -> graph is connected (not connected -> does not have a HP)
2. Being a complete graph is sufficient condition to have a HP
	- Complete -> HP
3. If G is a connected graph with |V| > 1 then all vertices have even degree is a necessary and sufficient condition for G to have an Euler Circuit
	- G connected, not singleton graph:
		- all vertices have even degree <-> EC




## Necessary conditions of having a HP
### Theorem 6.4.1
If G is a graph with Hamiltonian cycle, then G-v is connected for every vertex in V
- Other words: Remove an vertex from G, the graph remains connected
- HC -> G-v connected
##### Proof
- G has a HC, call it C.
- For any vertex, C-v is a path through all vertices in V-{v}. So G-v is connected.
- Done

##### Example: ![[Pasted image 20231126140505.png]]
- Since G-v is disconnected, then G doesn't have a HC to begin with

### Theorem 6.4.2
If a bipartite graph, then the size of the to sides must be the same. If |V1| = |V2|
##### Proof: ![[Pasted image 20231126140639.png]]
- A HC has the form: v1-w1-v2-w2-v3-w3 ... vk-wk-vi
	- These have to occur in pairs
		- Because they happen in pairs, the size of both vertex sets must be the same

###### Example: K2,3 does not have a HC
- because 2 =/= 3




### A sufficient condition to have a HP
Theorem 6.4.3
Let G be a graph with |V| = n
If
deg(x) + deg(y) >= n-1 for all x,y in V with x =/= then G has a Hamiltonian Path (Assumption 1)

Proof:
We start by showing that Assumption 1 implies G is connected.
	Claim: By Assumption 1, G is connected.
<span style="color:#0070c0">
Proof: Towards a contradiction suppose G is not connected. Let V1 and V2 be vertices 
		in different components, say H1 and H2. Let n1= |V(|H1)|(number of vertices in H1), n2 = |V(H2)| (Number of vertices in H2), then n1 + n2 <= n.
		deg(v1) + deg(v2) >= n - 1 (from Assumption 1)
			But, deg(v1) + deg(v2) <= n1 -1 + n2 - 1 = n- 2 (this contradicts Assumption 1)
				v1 is in a component with n1 vertices, biggest degree it can have, connected to all n1 - 1 vertices, so at most n1-1
			This contradicts Assumption 1. </span>
	<span style="color:#ffc000">Now we show G has a HP.
	Consider a path of maximum length:
		Path P: V1--------V2------V3------ ..... -----Vm-1------Vm
	Have 2 cases to consider.
	1. P contains all vertices in G. Then we are done. P is a HP
	<span style="color:#c00000">2. Other, P does not contain at least one vertex from G. This means *m* < *n*
	</span>
	<span style="color:#0070c0">Claim: By Assumption 1, there is a cycle containing {v1,v2,...,vm}
	Proof: Since P is maximal (can't be extended), v1 and vm are adjacent only to vertices on the path. (V1 and VM must be able to get to other vertices, can't extend because its already maximal)
	- If {v1,vm} is in G, then we are done
		- ![[Pasted image 20231127144515.png]]
	- Else if v1 is incident with Vi and vm is incident with vi-1 then we have a cycle as desired
		- ![[Pasted image 20231127144617.png]]
			- Could just delete the edge between vi-1 and vi
				- still have a cycle
	- Else V1 is incident with k vertices, then vm is incident with m-1-k vertices So then
		- deg(v1) + deg(vm) <= k + (m-1) -k
										- <= m -1
										- < n-1
										- This contradicts Assumption 1
	</span>
	
	</span>
	 

