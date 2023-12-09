- Objective:
	- detect faults due to interface errors/invalid assumptions about interfaces
- Interface types:
	- Parameter interfaces Data passed from one method/procedure from another
	- Shared memory interfaces Block of memory is shared between procedures or functions
![[Pasted image 20231209005447.png]]

#### Interface Errors
- [[Interface Misuse]]
- [[Interrace misunderstanding]]
- [[Timing errors]]

#### Testing Guidelines
- Use extreme value parameters to called procedures
- Always test pointer parameters with null pointers
- Design test which cause the component to fail
- Use stress testing in message passing system
- In shared memory system, vary the order in which components are activiated