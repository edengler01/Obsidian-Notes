**Intro**
- Programs are math objects
	- Should it not be possible for us to prove them?


**What can we prove?**
- Manual proofs are limited to programs of small size
- People who prove programs restrict the size of the program they can handle
	- Which is orders of magnitude different from the size of a battle-management system



**Do we have specifications?**
- In terms of SDI, no proof could be applied 
	- size is not the problem
	- its the lack of specifications
	- If we wrote a formal spec for it, have no way of telling what it can do

**Can we have faith in proofs**
- Proofs may help increase confidence
	- but not completely
- Reliable when they are small, well polished and carefully read
	- Not when they are large, complex and only read by the author

**What about concurrency?**
- Proofs practical to sequential programs
- Some techniques can be applied for shared memory
	- but more difficult


**What about programs that are suppose to be robust?**
- One major problem
	- SDI needs to function when part of it is disabled by the enemy
- Incredibly rare for program to give correct answer when suffering from a hardware failure.
- We have no way to proof if a program can run correctly in the event of partial failure

**Conclusion**
- No way to provide a proof of correctness for a small portion of the SDI