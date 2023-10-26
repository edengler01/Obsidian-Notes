**The Conventional Method**
"Think like a computer". Think what the computer would first do and then do the algorithm step-by-step until the task is done. 

**How does this lead to confusion**
Only works on small problems that don't matter. Once the program depends on conditions that are not known until runtime, we must deviate from this method. As soon as loops are involved, it becomes complex as we have to remember where we are. We need to keep track of earlier states as well. The amount of info we need to remember grows exponentially. 
The simple rules begin to grow in to something too complex for the human mind and we eventually make an [[error]]. Once one error is fixed, many new problems may be created.

**What is the effect of concurrency of this method**
If sequence of tasks being completed can not be anticipated, then the computers behaviour can not be anticipated as well. 
Computer may be doing one thing at a time, but there are many conditionals it needs to reach. Designing systems that try to anticipate the order the computer will run them leads to even more confusion.

**What is the effect of multiprocessing**
Software is just computer doing many things at once. There is no sequential program to study. Too many possibilities. 

**Do professional programmers really use this?**
They do. They at first try different approaches, but eventually degrade into the conventional way of thinking. 

**How do we get away with this inadequate approach?**
Programming is a trial and error craft. Spend as much time testing and debugging as they spent writing the program. Software is released when it is useable with very little bugs (not the absence).
Users learn to expect errors and are told how to avoid them.

**Conclusion**
Military software may not likely be correct. Methods that are used in the industry are not adequate for large real-time software systems that need to be reliable on first run. A drastic change is methods is needed. 