# 8.1 
i. The vertex set is {x<sub>1</sub>,x<sub>2</sub>,...,x<sub>k</sub>,} U {y<sub>2</sub>,y<sub>2</sub>,...y<sub>k</sub>}
ii. The edge set is {(x<sub>1</sub>,y<sub>1</sub>), (x<sub>2</sub>,y<sub>2</sub>,), .... , (x<sub>k</sub>,y<sub>k</sub>) }
<span style="color:#c00000">How many connected components are in the graph?</span>
- There are k components in the graph. There is an edge between every x<sub>i</sub> and y<sub>i</sub>
- The edge set of e<sub>k</sub> = {x<sub>i</sub>,y<sub>i</sub>} forms a component
# 8.2
If G = (V, E) is a graph with no loops such that |V | = v and |E| = e, prove that 2e ≤ v 2 − v.

Since G has no loops and the number of edges between two vertices ≤ 1, it follows that the number of edges in G denoted by e satisfies
e ≤ vC2 = v(v-1)/2 
Hence, 2e ≤ v<sup>2</sup> - v

# 8.3
Draw the multigraph G = (V, E) where V = {1, 2, 3, 4, 5} and E = {{1, 2}, {2, 3}, {2, 4}, {3, 1}, {3, 1}, {3, 3}, {4, 5}, {5, 5}, {4, 1}, {4, 3}} and list all cycles in G

Picture: ![[Pasted image 20231129154906.png]]
# 8.4
Let G be a connected multigraph with exactly two vertices of odd degree. Show that G has an Euler trail.


# 8.5 
(i) Does K4 have an Euler circuit? If yes, draw one. If not, explain. 
(ii) Does K4 have an Euler trail? If yes, draw one. If not, explain. 
(iii) Does K5 have an Euler circuit? If yes, draw one. If not, explain. 
(iv) Does K5 have an Euler trail? If yes, draw one. If not, explain.