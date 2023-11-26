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
		Proof: Towards a contradiction suppose G is not connected. Let V1 and V2 be vertices 
		in different components, say H1 and H2. Let n1= |V(|H1)|(number of vertices in H1), n2 = |V(H2)| (Number of vertices in H2), then n1 + n2 <= n.
		deg(v1) + deg(v2) >= n - 1 (from Assumption 1)
			But, deg(v1) + deg(v2) <= n1 -1 + n2 - 1 = n- 2 (this contradicts Assumption 1)
				v1 is in a component with n1 vertices, biggest degree it can have, connected to all n1 - 1 vertices, so at most n1-1
			This contradicts Assumption 1.
