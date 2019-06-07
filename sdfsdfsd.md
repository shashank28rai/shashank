# Garbage Collection generation

* The heap memory is divided into number of generations. 
* Normally it is three generations.
* The Generation 0 is for short live objects,.
* Generation 1 is for medium live objects which are moved from Generation 0. 
* Generation 3 is mostly stable objects. 
* When an object is created then it will allocate the memory space which will be higher.
* It will be in the Generation 0 and the memory allocation will be continuous without any space between the generations of garbage collectors.

## **How it works:-**

* Implicit Garbage Collection should be handled by the .Net framework. 
* When object is created then it will be placed in the Generation 0. 
* The garbage collection uses an algorithm which checks the objects in the generation, the objects life time get over then it will be removed from the memory. 
* The two kinds of objects. One is Live Objects and Dead Objects. 
* The Garbage collection algorithm collects all unused objects that are dead objects in the generation.
* If the live objects running for long time then based on that life time it will be moved to next generation.
* The object cleaning in the generation will not take place exactly after the life time over of the particular objects. 
* It takes own time to implement the sweeping algorithm to free the spaces to the process.

