### Definition: Euler Circuit
- A multigraph where every edge in *E* appears once in a Graph W and ends at the start point
		- |E| needs to be greater than or equal to 1
- ![[Pasted image 20231125021324.png]] 


#### Lemma
- Let G be a multigraph with |E| >= 1
- If deg(v) for all v in V, then G contains a cycle of length >= 1
	- <span style="color:#0070c0">If G has a loop, then it has a cycle of length >=1</span>
	- <span style="color:#c00000">If G does not have a loop, then it must have a path of at least one edge</span>
		- Let P be a path in G starting at vertex V0 and P is of maximum length (P cannot be enlarged). Since deg(vM)>=, then Vm must be incident to another edge
			- ![[Pasted image 20231125021623.png]]
		- Since P is maximal, the edge e must be included to any of the vertices 
	- Three case:
		- ![[Pasted image 20231125021709.png]]
		- Hence, we see that G has a cycle in case 3, we are done

### Theorem (Euler)
- A connected multigraph that is not a singleton vertex has a Euler circuit iff every vertex in V has even degree
	- <span style="color:#c00000">Proof</span>
			- Let G be a connected graph G, not singleton and has a Euler circuit
			- ![[Pasted image 20231125021910.png]]
	- Each time a walk happens, we use two edge. 
		- Every edge appears only one during a Euler walk
			- Then the degree of every vertex has to be even
	-  Use of induction on |E|
		- Induction
			- Base Case: |E| = 1
			- G = a loop
				- deg(v) = 2
				- G has a Euler circuit
		- Induction hypothesis (Consider |E| > 1)
			- Assume that given theorem is true for all graphs such that
				- 1 <= |E| <= n (number of edges)
			- Since G has even degree vertices and G is connected and deg(v) >= 2
			- We have that G has a cycle (say C) by the Lemma
			- Let {V1, V2,..Vm} be the vertices on that cycle C.
			- If C contain all edges in G, then we are done. Suppose that then there are edges in G but not in C

### Definition: Euler trail
- A multigraph where every edge appears once in T but ends at a different vertex than the start
	- ![[Pasted image 20231125022518.png]]
- Note: A graph that has a Euler trail will have exactly two vertices in G of odd degree