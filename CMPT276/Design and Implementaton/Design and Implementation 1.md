Gordon college ATM Example: [Wayback Machine (archive.org)](https://web.archive.org/web/20180822010044/https://www.math-cs.gordon.edu/courses/cs211/ATMExample/)

## From Code Complete
Design on Nondeterministic
- Can send 3 different people do design a program
	- 3 different ways
		- but all work
Design is a Heuristic Process
- Due to nondeterministic nature - techniques tend to be "rule of thumb"
- Involves trial and error
Design is Emergent
- Design isn't fully formed from the get go
	- its iterated on

Desirable Characteristics:
- Minimal complexity
- Ease of maintenance
- Loose coupling
- Extensibility
- Reusability
- High fan-in
- Low-to-medium fanout
- Portability
- Leanness
- Stratification
- Standard techniques




## Build or Buy
Domain
- Why reinvent the wheel?
	- If the software is out there, is it cheaper to just buy it instead of developing it?
### Commercial Off-The-Shelf
- software/hardware products ready-made for sale to the general public
	- Example: Microsoft Office



## Software Design Process Activities
![[Pasted image 20231207131813.png]]
### Structured methods
- Systematic approaches to software design
- usually a visual model
- Examples:
	- Object model
	- Sequence model
	- State transition model
	- Structural model
	- Data flow model

### Software Design Principles That Should be avoided
- Rigidity
	- Hard to change system as changes will have cascading effect
- Fragility
	- If changes are made, unexpected parts of the system break
- Immobility
	- Hard to reuse in another app because it cannot be disconnected to the current app


### Object Oriented Analysis
- Difference from other forms: requirements are organized around objects
	- which integrated both data and functions
	- Modelled after real-world objects that the system interacts with
- Traditional: Functions and data are considered separate


### Objected-Oriented Design Process
- Implements conceptual model during OOA
- Concepts are mapped onto implemented classes
- Constraints are identified
- Interfaces are designed
- Result: Model for the solution domain
	- e.g: a detailed description of how the system to be built on concrete technologies

##### Implementation details generally include:
- Restructuring class data
- Implementation of methods (internal data structures and data algorithms)
- Implementation of control
- Implementation of associations


##### Note on OOP
- Care more about the objects we want to manipulate
	- instead of the logic required to manipulate them

- The OOD process involves developing many different system models
	- Might not be feasible for small systems
	- Works for large systems
		- Important for communication
### Process Stages
- Variety of different processes
- Common activities <span style="color:#0070c0">(Weather station example)</span>
	- **Define context & models of use of the system**
		- Understand how the system is going to interact with out environment
		- Understand how the system is going to communicate with its environment
		- Understanding of the context helps establish limits of the system
			- Helps guide what features are going to work/not work
		- Context Model: shows how other systems in the environment of the system are being developed
		- Interaction model: dynamic model shows how the system interacts with its environment
	- **Design system architecture**
		- With interactions understood, use this info for design
		- Major components identified
	- **Identify key system objects**
		- Often difficult
		- Iterative process. Won't get it the first time
		- Approaches: natural language description, base off tangible things in domain, behavioral approach, scenario-based analysis
	- **Develop design models**
		- show objects and classes and relationships between them
		- 2 kinds
			- Structural Models: static structure of the system
			- Dynamic Models: describe dynamic interactions between objects
		- Examples: Subsystem model show logical groupings of objects into coherent subsystems
			- Sequence: show object interactions
			- State machine: show how individual objects change their state in response to events
			- Other: use-case, aggregation, generalization
	- **Specify object interfaces**
		- Object interfaces have to be speicifed
			- Objects and other components can be designed in parallel
		- Avoid designing it directly
			- Hide this into the object itself
		- Objects may have several interfaces
		- UML can be used for interface specification
Context
Interaction Models


## Design Models

