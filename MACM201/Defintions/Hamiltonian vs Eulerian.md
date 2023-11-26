Hamiltonian: Each vertex appears exactly once
Eulerian: Each edge appears exactly once.
- Having a Hamiltonian cycle and having an Euler circuit is very different


For testing if a graph has an Euler circuit:
- The fast algorithm: Linear function of |V| + |E| 
	- Test if G is connected and all vertices have even degree

No fast test for Hamiltonian cycle
- Currently NP complete