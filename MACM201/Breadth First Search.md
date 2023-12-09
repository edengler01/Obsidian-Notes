## Idea
- Fan out. Repeat at new vertex


## Algorithm
![[Pasted image 20231203000217.png]]
Using a queue structure, insert vertices into it

Step 1. Insert root vertex (1) in to Q
- Q = {1}
Step 2. Pop the vertex and add its neighbors to the queue
- Q = {2 4}
- Add to edge set, E<sub>t</sub> = (1,2), (1,4)
Step 2. Pop 2. Add its neighbors: 5 3 7
- Q = {4 5 3 7}
- Add to edge set, E<sub>t</sub> = (2,3), (2,5) (2,7)

Step 3. Pop 4. Add its neighbor: 6
- Q = {5 3 7 6}
- Add to edge set, E<sub>t</sub> = (4,6)


## Resulting Spanning Tree
![[Pasted image 20231203001711.png]]