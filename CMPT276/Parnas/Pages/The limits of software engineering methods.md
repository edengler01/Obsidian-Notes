**What is software engineering research?**
Common goal in this research is to reduce the amount the programmer must remember when testing a program.

Two main lines of research are
1. Structured programming and the use of formal program semantics.
2. The use of formally specified abstract interfaces to hide information about one module.
Third idea, less understood, is the use of cooperating sequential processes to help deal with the complexities arising from concurrency and multiprogramming.

There was a large gap between theory and practice.
The Software Cost Reduction project was expected to take two to four years, yet exceeded that deadline. It made two things clear
1. Much of what academic proposed can be done.
2. Good SWE is far from easy. They reduce the need for testing.

**What should we do and can do?**
SCR Project based on these precepts:
1. Requirements should be clear with complete, black-box requirements document before development begins.
2. System should be divided into modules using information-hiding (abstraction) before coding 
3. Each module should have a precise, black-box formal specification before coding
4. Formal methods should be used to give precise documentation
5. Real-time systems should be built as a set of cooperating sequential processes, each with a specified period and deadline.
6. Programs should be written using the ideas of structured programming taught by Harlan Mills



**What makes SWE hard?**
Hard to make decisions when we haven't played with the system yet. Only when something similar is built is it easy to determine the requirements. 
We know how to make abstract interfaces. Its hard to determine the right interface.
The common thread in all of these observations is that we need experience with similar systems to design reliable software. 

**Will new programming languages make much difference?**
Things like UNIX have made small improvements by eliminating some not needed processing tasks, but nothing substantial. Environments are not the crux of the SCR problems.

**Why software engineering research will not make SDI goals attainable**
SWE methods do not eliminate errors. Does not remove the basic differences between engineering and software technology, nor extensive testing under certain conditions. Successful application of methods is based off of previous experience from similar systems, which is not applicable to something new like SDI battle management.

**Conclusion**
Research may still no be able to change the fact that its hard to make a system without previous data to go off, despite having all the resources.
