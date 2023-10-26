**Preamble**
Most engineering products that have been completed, test and sold have a reasonable assumption that the design is correct and works reliably.
However it is not the case with software as it has some major bugs and affects some users.


**System Types**
Can be classified in three categories
1. [[Discrete State Systems]]
2. [[Analog Systems]]
3. [[Hybrid Systems]]

**Math Tools**
[[Analog Systems]] form the core of traditional engineering. Continuous functions in mathematics are well understood. We are saying that a system should not contain any hidden surprises. Engineers aim to create a [[Reliable System]].

Before digital computers, number of states in [[Discrete State Systems]] were small, so they could be tested exhaustively. Due to being so small, math tools were not needed to correct as people had systematic ways to determine behaviour.

[[Hybrid Systems]] can be verified using a combination of both methods. We can create a finite subset of operating states for discrete behaviour. Within those states, they can be described continuously. Usually these number of states are small. For each states, an analysis tool is used.

With the size of [[Discrete State Systems]] increasing, a very large of number of states started appearing. Systems comprised of copies of smaller systems, which can be analyzed and tested. Due to the amount of copied systems, large amounts of testing was not required.
- Design errors could be found in hardware, but they were deemed exceptional as they did not occur in repetitive structures

Software lacks the repetitive structure of hardware. Number of states are exponentially larger than nonrepetitive states of hardware. Traditional engineering math does not help in verification.

**How can we understand software?**
To make this situation better, two techniques
1. [[Build software in highly organized collection of small programs]]
2. [[Use of math logical to replace continuous math]]

**Education of Programmers**
Most traditional engineers have been educated to understand the math tools that are available to them.
Most programmers can not begin to use the tools that are available to them
