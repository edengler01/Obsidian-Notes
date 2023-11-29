# 9.1
Drawing a planar dual algorithm.
- In the original graph, place a vertex in the each face of the graph.
- Then make sure at lease one edge of the dual graph intersects with the original graph
# 9.2
If a connected graph has 20 vertices and 37 edges, how many faces will there be in a plane embedding?
- We can use [[Euler's Formula]]
- Plugging the values in to the formula: 
	- 20 - 37 + |F| = 2
	- -17 + |F| = 2
	- |F| = 19
# 9.3
Let G be a connected graph embedded in the plane. Prove that G has even number of faces of odd degree. 
- Recall the [[degree sum formula]] for faces.
- If a list of integers has even sum, then the total number of odd integers must be even
	- Following from this, there must be an even number of odd faces
# 9.4
Let G be a connected graph embedded in the plain satisfying |E| = 3|V| - 6. Prove that every face of G has degree 3
- Since G is connected and satisfies |E| = 3|V| - 6 it must be |V| >= 3
- Since G is connected with at least 3 vertices and no loops or parallel edges, every face must have degree of at least 3. Let F be the set of Faces and assume F = {f <sub>1</sub>,...... f<sub>k</sub>} (so |F| = k). Then:
	- 2|E| = summation deg(f<sub>i</sub>) >= Summation 3 = 3|F|
	- Using this together with 3 times Euler's formula we have
		- 6 = 3|V| - 3|E| + 3|F|
# 9.5
# 9.6


