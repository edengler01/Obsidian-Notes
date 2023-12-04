# 10.1
![[Pasted image 20231128145634.png]]
Graph Website link: http://graphonline.ru/en/?graph=RfKVBUIWIKfXNnSj


### Graph
- ![[Pasted image 20231128225806.png]]

a) Check for [[Hamilton Cycle]]
- [[Necessary Conditions for Hamilton Cycle]]
	- Connected? Yes
	- No cut Vertices? (when a vertex is deleted, the graph is disconnected)``
	- No vertex with a degree < 2? (not a leaf or an end vertex)
Is it a Hamilton Cycle? <span style="color:#c00000">No</span>

b) Does it have a Hamilton Path? <span style="color:#00b050">Yes</span>
- ![[Pasted image 20231128154348.png]]


c) Does it have a spanning tree? DFS Spanning Tree?
<span style="color:#00b050">Yes</span>
![[Pasted image 20231128154651.png]]

# 10.2
![[Pasted image 20231128154736.png]]
![[Pasted image 20231128154806.png]]
The structure of a depth first search on K<sub>n,n</sub> will always be a [[hamilton path]]
It will start on one side of the partition and zig zag sides but will eventually use all the vertices


# 10.3
![[Pasted image 20231128154916.png]]
<span style="color:#0070c0">a)</span> If |V<sub>1</sub>| is less than 2, then G does not have a HC. If |V<sub>1</sub>| and |V<sub>2</sub>| are not equal then G could be the bipartite graph K<sub>2,3</sub> which does not have a HC. Therefor a is true.
<span style="color:#0070c0">b)</span> False. Consider a graph with V<sub>1</sub> = *{a.b}* and V<sub>2</sub> = *{c,d}* and E = *{(a, c), (b, c), (b, d)}*
- Clearly G is connected with |V<sub>1</sub>| = |V<sub>2</sub>| = 2 but G does not have a HC.

# 10.4
![[Pasted image 20231128215801.png]]
Let V<sub>1</sub> and V<sub>2</sub> be the bipartition of K<sub>n+1,n</sub>
|V<sub>1</sub>| = *n + 1*, |V<sub>2</sub>| = *n*
- Every HP will have to start and end in V<sub>1</sub>
- There are *n+1* ways to choose the first vertex (from V<sub>1</sub>) and *n* ways to choose the second vertex(from V<sub>2</sub>)
	- This process continues until the last vertex is chosen
		- *(n+1)! x n!* HP appear.
		- We need to divide by 2! as we are counting the reverse case as well
- Thus there are *((n+1) n!)/2! *

# 10.5
![[Pasted image 20231201174815.png]]
Consider the cycle on V = {1,2,3,4,5}. 
- Has a [[hamilton path]]
- deg(*x*) + deg(*y*) = 4 ≥ 5 - 1 = 4
But if the cycle on V = {1,2,3,4,5,6} and we consider a cycle on 6 vertices we have that
- deg(*x*) + deg(*y*) = 4 ≥ 6-1 = 5 which is not true
Which disprove the converse of the result