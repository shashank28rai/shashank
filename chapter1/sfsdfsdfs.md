# C \# Interview Questions and Answear 2

## **What is C-Sharp \(C\#\)**

C\# is a type-safe, managed and object oriented language, which is compiled by .Net framework for generating intermediate language \(IL\).

## **Explain the features of C\#**

Below are some of the features supported in C\# -

* Constructors and Destructors
* Properties
* Passing Parameters
* Arrays
* Main
* XML Documentation and
* Indexers

##  **List some of the advantages of C\#**

Below are the advantages of C\# -

* Easy to learn
* Object oriented
* Component oriented
* Part of .NET framework

###  **What are IDE’s provided by Microsoft for C\# development**

Below are the IDE’s used for C\# development –

* Visual Studio Express \(VCE\)
* Visual Studio \(VS\)
* Visual Web Developer

###  **Explain the types of comments in C\#**

Below are the types of comments in C\# -

* Single Line Comment Eg : //
* Multiline Comments Eg: /\* \*/
* XML Comments Eg : ///

###  **Explain sealed class in C\#**

Sealed class is used to prevent the class from being inherited from other classes. So “sealed” modifier also can be used with methods to avoid the methods to override in the child classes.

###  **Give an example of using sealed class in C\#**

Below is the sample code of sealed class in C\# -

```text
class X {} 

sealed class Y : X {}

Sealed methods –

class A
{
 protected virtual void First() { }

 protected virtual void Second() { }

}
class B : A
{
 sealed protected override void First() {}

 protected override void Second() { }

}
```

If any class inherits from class “B” then method – “First” will not be overridable as this method is sealed in class B.

###  **List out the differences between Array and ArrayList in C\#**

* Array stores the values or elements of same data type but arraylist stores values of different datatypes.
* Arrays will use the fixed length but arraylist does not uses fixed length like array.

### **Why to use “using” in C\#**

“Using” statement calls – “dispose” method internally, whenever any exception occurred in any method call and in “Using” statement objects are read only and cannot be reassignable or modifiable.

###  **Explain namespaces in C\#**

Namespaces are containers for the classes. We will use namespaces for grouping the related classes in C\#. “Using” keyword can be used for using the namespace in other namespace.

###  **Why to use keyword “const” in C\#? Give an example.**

“Const” keyword is used for making an entity constant. We can’t reassign the value to constant.

```text
Eg: const string _name = "Test";
```

###  **What is the difference between “constant” and “readonly” variables in C\#**

* “**Const**” keyword is used for making an entity constant. We cannot modify the value later in the code. Value assigning is mandatory to constant variables.
* “**readonly**” variable value can be changed during runtime and value to readonly variables can be assigned in the constructor or at the time of declaration.

###  **Explain “static” keyword in C\#**

“Static” keyword can be used for declaring a static member. If the class is made static then all the members of the class are also made static. If the variable is made static then it will have a single instance and the value change is updated in this instance.

### **What is the difference between “dispose” and “finalize” variables in C\#**

* **Dispose -** This method uses interface – “IDisposable” interface and it will free up both managed and unmanaged codes like – database connection, files etc.
* **Finalize -** This method is called internally unlike Dispose method which is called explicitly. It is called by garbage collector and can’t be called from the code.

### **How the exception handling is done in C\#**

In C\# there is a “try… catch” block to handle the error.

