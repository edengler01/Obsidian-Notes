**Preamble**
To create an ICBM defense system, need software so well-developed it could have extremely high confidence in working correctly

**Characteristics of a proposed battle management software system***
1. Able identify, track and direct weapons towards ICBMs that cannot be known with certainty before battle. Must be able to tell from decoys
2. Computing done by network of sensors, weapons and each other, where behaviour can not be anticipated by the enemy to prevent use of countermeasures. 
3. Impossible to test the system under real conditions prior to actual use
4. Short service period, little human intervention and no chance to debug and modify program on the fly
5. Absolute real time deadlines for computations. Computational processes cannot be predicted in advance due to target changing characteristics
6. Ever increasing suite of weapon systems, which are also built on large and complex systems. Increasing complexity of the entire battle defense system

**Implications of these problem characteristics**
1. Fire control software can not be written without making assumptions about the target. Assumptions needed in algorithms for determine with target is hostile or not. If software has no assumptions, enemy can change characteristics day of launch.
2. No success except for certain situations such as incidents based off past history , failures are unlikely, excess capacity, real-time deadlines are soft
3. No large scale system has been installed without extensive testing under realistic conditions. Inability to test defense system mean that no one could gauge how much faith they can have in the system
4. Not unusual for software mods on the fly
5. Must meet hard real-time deadlines reliably. Theoretically done at runtime or pre runtime scheduling. However no one for sure can determine whether it can meet those deadlines 
6. Problems worsen when interfaces change. Difficulties increase when increasing size of systems

**Conclusion**
It will cost a lot. Numerous characteristics make it hard to test, leading to not having much faith in the system. This is all not taking size into account.