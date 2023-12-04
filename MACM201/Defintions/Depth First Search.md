## Idea
- Starting at the root vertex, we traverse as far as we can, then back track when we hit a dead end

## Algorithm
![[Pasted image 20231202235119.png]]
Step 1: Starting at vertex 1 (root), look at its neighbor and traverse to the smallest one
- Look at 2 & 4. Which is smaller: 2. Traverse to 2.
Step 2: Starting at vertex 2, look at children 5, 3, 7. Which is smaller: 3
Step 3: At vertex 3, look at children 5,7. Which is smaller: 5
Step 4: At vertex 5, look at children. 2 has been visited. Back track to previous vertex
Step 5: At vertex 3, look at children. 7 hasn't been visited. Move to 7
Step 6: At vertex 7, look at children. 2 has been visited. 4 has not. Move to 4
Step 7: At vertex 4, look at children. 1 has been visited. 6 has not. Move to 6
Step 8: At vertex 6, look at children. It has no children. Back track
*Backtracks until the root has been reached*
If back track back to root, we are done.
For each step, Edge set is tracked.

E<sub>t</sub> = {(1,2), (2,3), (3,5), (3,7), (7,4),(4,6)}


## Resulting Spanning Tree
![[Pasted image 20231203001739.png]]