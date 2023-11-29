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


# 10.3
![[Pasted image 20231128154916.png]]
Sufficient Condition <span style="color:#c00000">A</span> is sufficient condition for <span style="color:#ffc000">B</span> whenever the occurrence of A is all that is needed for the occurrence of <span style="color:#ffc000">B</span>

Necessary Condition: <span style="color:#ffc000">B</span> is a necessary condition for <span style="color:#c00000">A</span> whenever <span style="color:#c00000">A</span> cannot occur without the occurrence of <span style="color:#ffc000">B</span>

To be both Necessary and Sufficient, 
a) We know that this is a necessary condition. We know that in a HC, the walk happens in pairs. 
- The HC has the form v<sub>1</sub> - w<sub>1</sub> - v<sub>2</sub> - w<sub>2</sub> ... w<sub>n</sub>-v<sub>n</sub>-v<sub>1</sub>
b) Note there are no necessary and sufficient 

# 10.5
![[Pasted image 20231128215801.png]]
We know that the left side will have n+1 vertices
We know that the right will have n vertices

We know for v<sub>1</sub> is n + 1 choices to pick
- To pick for v<sub>2</sub>, we will have n choices
- For each subsequent vertex, there will be n choices
So there will be (n+1) x n<sup>n</sup>
- Picture: ![[Pasted image 20231128222839.png]]
- 