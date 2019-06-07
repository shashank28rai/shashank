# C \# Interview Questions and Answear 1

## **Can we execute multiple catch blocks in C\#**

No. Once any exception is occurred it executes specific exception catch block and the control comes out.

##  **Why to use “finally” block in C\#**

“Finally” block will be executed irrespective of exception. So while executing the code in try block when exception is occurred, control is returned to catch block and at last “finally” block will be executed. So closing connection to database / releasing the file handlers can be kept in “finally” block.

##  **What is the difference between “finalize” and “finally” methods in C\#**

* **Finalize –** This method is used for garbage collection. So before destroying an object this method is called as part of clean up activity.
* **Finally –** This method is used for executing the code irrespective of exception occurred or not.

##  **What is the difference between “throw ex” and “throw” methods in C\#**

* “**throw ex**” will replace the stack trace of the exception with stack trace info of re throw point.
* “**throw**” will preserve the original stack trace info.

##  **Can we have only “try” block without “catch” block in C\#**

Yes we can have only try block without catch block.

##  **List out two different types of errors in C\#**

Below are the types of errors in C\# -

* Compile Time Error
* Run Time Error

##  **Do we get error while executing “finally” block in C\#**

Yes. We may get error in finally block.

##  **Mention the assembly name where System namespace lies in C\#**

Assembly Name – mscorlib.dll

##  **What are the differences between static, public and void in C\#**

* Static classes/methods/variables are accessible throughout the application without creating instance. Compiler will store the method address as an entry point. 
* Public methods or variables are accessible throughout the application. 
* Void is used for the methods to indicate it will not return any value.

##  **What is the difference between “out” and “ref” parameters in C\#**

“**out**” parameter can be passed to a method and it need not be initialized where as “**ref**” parameter has to be initialized before it is used.

##  **Explain Jagged Arrays in C\#**

If the elements of an array is an array then it’s called as jagged array. The elements can be of different sizes and dimensions.

##  **Can we use “this” inside a static method in C\#**

No. We can’t use “this” in static method.

##  **What are value types in C\#**

Below are the list of value types in C\# -

* decimal
* int
* byte
* enum
* double
* long
* float

##  **What are reference types in C\#**

Below are the list of reference types in C\# -

* class
* string
* interface
* object

##  **Can we override private virtual method in C\#**

No. We can’t override private virtual methods as it is not accessible outside the class.

