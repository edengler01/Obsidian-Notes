
##  [Equivalence Partitioning](https://testsigma.com/blog/equivalence-partitioning/)
- Black-box testing techinque
- Allows testers to group input data in categories
	- Makes it possible reduce number of test cases
	testsigma.com/blog/equivalence-partinioning

## Testing Guidelines
- Test software with sequences of singular value
- Use obvious cases (such as initial case, 0th case, extreme case)
- Why?
	- Can't test exhaustvely
		- impossible for software


If input is too big
	becomes intractable
	Weather is an example

## General Guidelines
- Chose inputs that force an error to show
- Design input to cause buffers to overflow
- Repeat the same input or series numerous times
- Force invalid outputs to be generated
- Force computation results to be extreme

confirmation bias in swe
	when testing, you aim to not break code

## Component Testing
- Software components are comprised of components that are also made up of several interacting objects
	- Weather station system
		- reconfiguration component includes objects that deal with each aspect of the reconfiguration
- Testing composite components should therefore focus on show that the component interface behaves according to its specification


## Interface Testing
- Objectives are to detect faults due to interface errors or invalid assumptions about interfaces
- Interface types
	- Parameter data passed from one method to another
	- Shared memory blocks between functions/procedures
	- Procedural interafce sub-system encapsulates a set of procedures to be called by other sub system
	- Message passing interfaces Sub-systems request services from other sub-systems
- ## Errors
	- [[Interface Misuse]]
	- [[Interface Misunderstanding]]
	- [[Timing errors]]
- ## Guidelines
	- Use extreme values for test parameters
	- Always test pointer parameters with null pointers
	- Design test which cause the component to fail
	- Use stress testing in message passing systems
	- In shared memory systems, vary the order in which components are activated

## System Testing
- involves testing during the development process
	- integrating components to create a version of the system and then testing said integrated system
	- Focus: test interactions between components
	- Checks if they are compatible, interact correctly, transfer the right data at the right time across their interfaces
	- System testing test the emergent behavior of a system

### System & Component Testing
- Reusable components that have been modified may be integrated with newly developed components
	- Complete system can then be tested
- Components can be developed by different team members or sub-teams
	- System testing is a collective process, as opposed to an individual process


### Use - Case Testing (good for presentation)
- Help identify system interactions that can be used as a basis for system testing
- Each use case usually involves several system components
	- Testing the use case forces these interactions to occur
- Sequence diagrams associated with the use case documents the components and interactions that are being tested
	
	

### Test Cases Derived from Sequence Diagram


# Test driven development
- The approach in which you inter weave testing and code development
- Tests are written before code and "passing" the tests are the main driver of development
- Develop code incrementally, along with the tests
	- Don't start development on the next increment until all tests have passed
- Was introduced as part of agile methods such as [[Extreme programming - XP]]
	- Can also be used in [[Plan-driven development]]
## Flow of Test Driven Development
![[Pasted image 20231122152157.png]]
## Process Activities
1. Start by dividing functionality into increments
	- should be small and implementable 
2.  Write a test for this small segment
3.  Run all tests
4. Then incrementally develop the functionality
5. Once all tests are successful, move to the next chunk


### Benefits
- Code Coverage
- Regression Testing
- Simplified Debugging
- System Documentation

## Regression testing


release testing


requirements based testing

Read: Slide 97

feature test by scenario

user testing
	Types

Acceptance testing
	stages
	Agile methods


	Software testing myth


CIO Cheat Sheet
