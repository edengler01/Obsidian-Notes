### Design Patterns
- a general repeatable solution to a commonly occurring problem in software design
- Design pattern: isn't a finished design that can be transformed into code
	- Its a description/template on how to solve a problem

- A way of reusing abstract knowledge about a problem & its solution
- Description of the problem & the essence of its soultion
- Should be sufficiently abstract show it can be reused in similar situations in a different setting
- Usually make use of OO characteristics such as inheritance & polymorphism

### Patterns
- ways to describe best practices, good designs, and capture experience for others to reuse

#### Elements
- Name
	- A meaningful pattern identifier
- Problem description
- Solution description
	- Not a concrete design but a template for a solution that can be implemented in different ways
- Consequences
	- Results and trade-offs in applying this pattern
#### The Observer Pattern
- Name
	- Observer
- Description
	- Separates the display of object state from the object itself
- Problem description
	- Used when multiple displays of state are needed
- Solution description
	- UML description
- Consequences
	- Optimizations to enhance display performance are impractical 

## Design Problems
- To use patterns in design, need to recognize that any design problem may have an associated pattern that can be applied
	- Tell several objects that the state of some other object has changed (Observer pattern)
	- Tidy up interfaces to a number of related objects that have been often developed incrementally (Facade Pattern)
	- Provide a standard way of accessing elements in collection, regardeless of how that collection is implemented (Iterator pattern)
	- Allow for possibility of extending the functionality of an existing class at run-time (Decorator pattern)

## Non-Programming Implementation Issues
- Reuse: Most modern software is constructed in reuse of components/systems. Try and make use of lots of existing code
- Config Management: Have to keep track of different version of each component. 
- Host-target development: Production software does not usually execute on the same computer
	- You develop it on one computer and execute it on a separate computer (host system vs target system)


## Reuse Levels
- **Abstraction level**: reuse knowledge of successful abstractions in the design
- **Object level**: directly reuse objects from a library
- **Component level**: collections of objects and classes that you reuse in application systems
- **System level**: Reuse entire applications systems

## Config Management
- Process of managing a changing software system
- Supports system integration process
	- so developers can access the project code/documents in a controlled way, see changes, compile and link components to create a system
### Activities
- Version management: support is provided to keep track of different versions of software components
	- Systems include facilities to coordinate development by several programmers
- System integration: Help developers define what versions of components are used to create each version of a system.
	- Description is used to build a system automatically by compiling and linking the required components
- Problem tracking: Allows users to report bugs & other problems
	- Allows developers to see who is working on the problems & when they are fixed


## Host-Target Dev
- Software mostly developed on one computer(the host), but runs on a separate machine (the target)
- Development platform vs Execution platform
	- Platform: more than just hardware
	- Includes OS, other software such as DBMS or an interactive development environment
- Dev platform usually has different installed software than execution platform
	- these platforms may have different architectures
![[Pasted image 20231207141553.png]]

## Dev Platform tools
- Integrated compiler & syntax-directed editing system
	- Create, edit, compile code
- A language debugging system
- Graphical editing tools
	- tools to edit UML models
- Testing tools (like JUNIT)
- Project support tools that help organize code for different development projects (like GitHub)

### IDE
- not compilers
- Software development tools are often grouped to create an integrated development environment (IDE)
- Set of software tools that support different aspects of SW development within some common framework and user interface
- Created to support development in specific programming language such as Java
	- Language IDE may be develop specifically or may be an instatnitaion of general purpose IDE, with specific language-support tools



# Open Source Development
- process where open-source software has their source code publicly available
## Issues
- should the product that is being developed make use of open source components?
- should an open source approach be used for the software's development
## Open Source Business
- More companies are using open source approach
- Model is not reliant on selling software
	- but selling support for that product
- Believe that involiving the open soruce community will allow software to be created cheaply, quickly and create a community of users for the software


## Licensing
- Fundamental Principle: Source code should be freely available
	- Does not mean anyone can do anything with that code
		- Legally: Dev of the code still owns it. They can place restrictions on how its used by including legally binding conditions in the open source software license
		- Some believe that if open source is used to develop a new system
			- that system too should be open source
		- Others willing to allow their code to be used with this restrictions
			- Developed systems may be proprietary and sold as closed source systems

## License Models
- GNU General Public License
	- If you use open source software using this license
		- Your software must be open source as well
- GNU Lesser General Public License
	- Can write components that link to open source code without having to publish the source of these components
- Berkley Standard Distribution License
	- Non reciprocal
	- Not obliged to re-publish any changes or modifcations made to open source code.
		- You can include the code in proprietary systems that are sold

## License Management
- Establish a system for maintaining info about open-source components that are downloaded and used
- Be aware of different types of license
	- Understand how a component is license before it is used
- Be ware of evolution pathways for components
- Educate people about open source
- Have auditing systems in place
- Participate in the open source community
