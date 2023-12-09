## Program Testing Goals
- [[Validation Testing]]
- [[Defect Testing]]

### Software Testing & Verification
[[Verification]] vs [[Validation]]
![[Pasted image 20231208232950.png]]
#### Note: "V & V Confidence"
- Aims to establish confidence that the system is "fit for purpose"
- Depends on:
	- [[Software purpose]]
	- [[User Expectation]]
	- [[Marketing environment]]

#### Software Testing Principles
- There is no universal agreement
- But there are "[[seven testing principles]]"
____
## Inspections & Testing
[[Software Inspection]] vs [[Software Testing]]
- Are complementary to each other
- Both should be used during the V & V process
- Inspections check conformance with a specification
	- but not the customer's real  [[functional requirements]]
	- Cannot check [[non-functional requirements]] characteristics such as performance, usability

_____

## Software Release Cycle
- The sum of stages of development and maturity for a piece of software
	- Ranges from intial development to initial release
	- Includes updated version of the released version to improve software or fix bugs

#### Three Testing Stages
1. [[Pre-alpha testing]]
2. [[Alpha testing]]
3. [[Beta Testing]]

#### Stages of Testing
- Development Testing ([[Pre-alpha testing]]): system is tested during development to discover bugs/defects
- Release testing: separate testing team test a complete version before it is released to users
- User testing ([[Alpha testing]], [[Beta Testing]]): users or potential users of a system test the system in their own environment

____

## Development Testing
- Includes all testing activities that are carried out during development
- [[Unit testing]]
- [[Component testing]]
	- [[Interface testing]]
- [[System testing]]
	- [[System and Component Testing]]
____
## Testing Strategies
- [[Partition testing]]
	- [[equivalence partition]]
- [[Guideline-based testing]]
____
## Testing Guidelines
- Test software with sequences of singular value
- Use obvious cases (such as initial case, 0th case, extreme case)
- Why?
	- Can't test exhaustively
		- impossible for software
- If input is too big
	- becomes intractable
	- Weather is an example

### [[Testing Policies]]
____
## General Guidelines
- Chose inputs that force an error to show
- Design input to cause buffers to overflow
- Repeat the same input or series numerous times
- Force invalid outputs to be generated
- Force computation results to be extreme
##### Note
- Confirmation bias in SWE
	- When testing, you aim to not break code
______
## Use - Case Testing (good for presentation)
- Help identify system interactions that can be used as a basis for system testing
- Each use case usually involves several system components
	- Testing the use case forces these interactions to occur
- Sequence diagrams associated with the use case documents the components and interactions that are being tested
____
# [[Test-Driven Development]]
- The approach in which you inter weave testing and code development
- Tests are written before code and "passing" the tests are the main driver of development
- Develop code incrementally, along with the tests
	- Don't start development on the next increment until all tests have passed
- Was introduced as part of agile methods such as [[Extreme programming - XP]]
	- Can also be used in [[Plan-driven development]]
## Flow of Test Driven Development
![[Pasted image 20231122152157.png]]
### [[TDD Process]]
### [[TDD Benefits]]


## [[Release Testing]]
- Release testing is a form of [[System testing]]
- [[Release testing vs System testing]]

## [[Requirements-Based Testing]]

## [[Performance Testing]]

## [[User Testing]]

## Summary
- Testing only show presence of errors in program
	- Does not show that there are no remaining faults
- Dev testing: responsibility of the dev team
	- Separate  team should be responsible for testing a system before it is released
- Dev testing includes;
	- [[Unit testing]]
	- [[Component testing]]
	- [[System testing]]
- Try to "break" the software
	- from cases that you have come across and [[Guideline-based testing]]
- Wherever possible
	- write utilize [[Test Automation]]
- Utilize [[Test-First Development]]
- Scenario testing involves inventing a typical usage scenario & using this to derive test cases
- Utilize [[Acceptance testing]]
Read: Slide 97

feature test by scenario



Acceptance testing
	stages
	Agile methods


	Software testing myth


CIO Cheat Sheet
