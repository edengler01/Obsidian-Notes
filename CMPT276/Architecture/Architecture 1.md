## Computer Architecture
- a set of rules & methods that describe the functionality, organization and implementation of computer system
- the fundamental structures of a software system, the discipline of creating them, and documentation

### Example
- [[Space Shuttle]]
- ![[Pasted image 20231110103120.png]]



## Advantages of Explicit Architecture
-  [[Stakeholder communication]]
- [[System analysis]]
- [[Large-scale reuse]]


## Architectural Representations
- Simple diagrams showing entities & relationships used frequently
	- but been criticized because they:
		- lack semantics
		- do not show types of relationships
		- show visible properties of entities
- Requirements for model semantics depend on how the models are used
## Box and Line Diagrams
- Very abstract
	- doesn't show nature of component relationships
	- doesn't show visible properties of sub-systems
- Useful for communication & project planning

## Use of Architectural Models
- To start a conversation about the system design
	- Stakeholders can understand and relate to the abstract view of an otherwise complicated system
- To document the architecture that has been design
	- aims to produce a complete system model that shows the different components in the system, their interfaces and their connections
## Architectural Design
#### Design Decisions
- Creative process
	- can differ depending on the type of system being developed
- Number of common decisions span all design processes
	- they can affect the non-functional characteristics of the system
- ![[Pasted image 20231110104910.png]]
#### Reuse
- Systems in the same domain often have similar architectures that reflect the concepts in that domain
- Apps product lines are built around a core
	- with variants that satisfy specific customer requirements
- Architecture of a system may be designed around one or more patterns or "styles"
	- capture the essence of an architecture and can be instantiated in different ways

#### System Characteristics
- [[Performance]]
- [[Security]]
- [[Safety]]
- [[Availability]]
- [[Maintainability]]
#### Views
- Questions to ask:
	- What views/ perspectives are useful when designing or documenting a system's architecture?
	- What notation should be used?
- Each model only shows one view or perspective of the system
- ![[Pasted image 20231110110228.png]]
- [[4 + 1 View Model]]

#### Representing Architectural Views
- Some argue that UML is appropriate for documentation
	- Sommerville disagrees as it does not believe UML includes abstractions appropriate for higher-level system descriptions
- [[ADLs]] have been developed but not widely used



