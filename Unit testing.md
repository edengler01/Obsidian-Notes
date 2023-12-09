- Individual program units/object classes are tested
- Unit testing should focus on testing the functionality of objects or methods
- A defect testing process
- Units may be:
	- Individual functions/methos within an object
	- Object classes with several attributes & methods
	- Composite components with defined interfaces used to access their functionality 

### Object Class Testing
- Complete test coverage of a class involves
	- Testing all operations associated with the object
	- Setting & retrieving all object attributes
	- Exercising the the object in all possible states
- Inheritance makes it difficult to design object class tests
	- Infor to be tested is not localized

### Automated Testing
- Make use of test automation framework (i.e, JUnit) to write & run program test
	- Provides generic test classes that you extend to create specific test cases
		- Can run all of the tests that you have implemented & report
			- Often through some GUI, on the success of otherwise of the tests

### Parts
1. Setup part: initialization of the system with test case (inputs and expected outputs)
2. Call part: object/method is called to be tested
3. Assertion part: Comparison of result of call with expected result
	- If assertion evaluates true, the test has been successful
	- If it fails, then test has failed
 
