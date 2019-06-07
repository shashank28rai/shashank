# C \# Interview Questions and Answear 3

## **Explain access modifier – “protected internal” in C\#**

“protected internal” can be accessed in the same assembly and the child classes can also access these methods.

## **In try block if we add return statement whether finally block is executed in C\#**

Yes. Finally block will still be executed in presence of return statement in try block.

## **What you mean by inner exception in C\#?**

Inner exception is a property of exception class which will give you a brief insight of the exception i.e, parent exception and child exception details.

##  **Explain String Builder class in C\#?**

This will represent the mutable string of characters and this class cannot be inherited. It allows us to Insert, Remove, Append and Replace the characters. “ToString\(\)” method can be used for the final string obtained from StringBuilder. For example,

```text
StringBuilder TestBuilder = new StringBuilder("Hello");

TestBuilder.Remove(2, 3); // result - "He"

TestBuilder.Insert(2, "lp"); // result - "Help"

TestBuilder.Replace('l', 'a'); // result - "Heap"
```

##  **What is the difference between “StringBuilder” and “String” in C\#?**

* StringBuilder is mutable, which means once object for stringbuilder is created, it later be modified either using Append, Remove or Replace.
* String is immutable and it means we cannot modify the string object and will always create new object in memory of string type.

##  **What is the difference between methods – “System.Array.Clone\(\)” and “System.Array.CopyTo\(\)” in C\#?**

* “CopyTo\(\)” method can be used to copy the elements of one array to other. 
* “Clone\(\)” method is used to create a new array to contain all the elements which are in the original array.

##  **How we can sort the array elements in descending order in C\#?**

“Sort\(\)” method is used with “Reverse\(\)” to sort the array in descending order.

##  **Explain circular reference in C\#?**

This is a situation where in, multiple resources are dependent on each other and this causes a lock condition and this makes the resource to be unused.

##  **List out some of the exceptions in C\#?**

Below are some of the exceptions in C\# -

* NullReferenceException
* ArgumentNullException
* DivideByZeroException
* IndexOutOfRangeException
* InvalidOperationException
* StackOverflowException etc.

##  **Explain Generics in C\#?**

Generics in c\# is used to make the code reusable and which intern decreases the code redundancy and increases the performance and type safety.  
Namespace – “System.Collections.Generic” is available in C\# and this should be used over “System.Collections” types.

##  **Explain object pool in C\#?**

Object pool is used to track the objects which are being used in the code. So object pool reduces the object creation overhead.

## **What you mean by delegate in C\#?**

Delegates are type safe pointers unlike function pointers as in C++. Delegate is used to represent the reference of the methods of some return type and parameters.

##  **What are the types of delegates in C\#?**

Below are the uses of delegates in C\# -

* Single Delegate
* Multicast Delegate
* Generic Delegate

## **What are the three types of Generic delegates in C\#?**

Below are the three types of generic delegates in C\# -

* Func
* Action
* Predicate

## **What are the differences between events and delegates in C\#?**

Main difference between event and delegate is event will provide one more of encapsulation over delegates. So when you are using events destination will listen to it but delegates are naked, which works in subscriber/destination model.

