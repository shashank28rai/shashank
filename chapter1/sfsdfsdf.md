# C \# Interview Questions and Answear 4

##  **Can we use delegates for asynchronous method calls in C\#?**

Yes. We can use delegates for asynchronous method calls.

##  **What are the uses of delegates in C\#?**

Below are the list of uses of delegates in C\# -

* Callback Mechanism
* Asynchronous Processing
* Abstract and Encapsulate method
* Multicasting

## **What is Nullable Types in C\#?**

Variable types does not hold null values so to hold the null values we have to use nullable types. So nullable types can have values either null or other values as well.

```text
Eg: Int? mynullablevar = null;
```

##  **Why to use “Nullable Coalescing Operator” \(??\) in C\#?**

Nullable Coalescing Operator can be used with reference types and nullable value types. So if the first operand of the expression is null then the value of second operand is assigned to the variable. For example,

```text
double? myFirstno = null;
double mySecno;
mySecno = myFirstno ?? 10.11;
```

##  **What is the difference between “as” and “is” operators in C\#?**

* “**as**” operator is used for casting object to type or class.
* “**is**” operator is used for checking the object with type and this will return a Boolean value.

## Define Multicast Delegate in C\#?

A delegate with multiple handlers are called as multicast delegate. The example to demonstrate the same is given below

```text
public delegate void CalculateMyNumbers(int x, int y);

int x = 6;
int y = 7;

CalculateMyNumbers addMyNumbers = new CalculateMyNumbers(FuncForAddingNumbers);

CalculateMyNumbers multiplyMyNumbers = new CalculateMyNumbers(FuncForMultiplyingNumbers);


CalculateMyNumbers multiCast = (CalculateMyNumbers)Delegate.Combine (addMyNumbers, multiplyMyNumbers);


multiCast.Invoke(a,b);
```

##  **What is the difference between CType and Directcast in C\#?**

* CType is used for conversion between type and the expression.
* Directcast is used for converting the object type which requires run time type to be the same as specified type.

## **Is C\# code is unmanaged or managed code?**

C\# code is managed code because the compiler – CLR will compile the code to Intermediate Language.

##  **Why to use lock statement in C\#?**

Lock will make sure one thread will not intercept the other thread which is running the part of code. So lock statement will make the thread wait, block till the object is being released.

##  **Explain Hashtable in C\#?**

It is used to store the key/value pairs based on hash code of the key. Key will be used to access the element in the collection. For example,

Hashtable myHashtbl = new Hashtable\(\);  
myHashtbl.Add\("1", "TestValue1"\);  
myHashtbl.Add\("2", "TestValue2"\);

##  **How to check whether hash table contains specific key in C\#?**

Method – “ContainsKey” can be used to check the key in hash table. Below is the sample code for the same –

```text
Eg: myHashtbl.ContainsKey("1");
```

##  **What is enum in C\#?**

enum keyword is used for declaring an enumeration, which consists of named constants and it is called as enumerator lists. Enums are value types in C\# and these can’t be inherited. Below is the sample code of using Enums

```text
Eg: enum Fruits { Apple, Orange, Banana, WaterMelon};
```

## **Which are the loop types available in C\#?**

Below are the loop types in C\# -

For  
While  
Do.. While

##  **What is the difference between “continue” and “break” statements in C\#?**

* “continue” statement is used to pass the control to next iteration. This statement can be used with – “while”, “for”, “foreach” loops.
* “break” statement is used to exit the loop.

##  **Write a sample code to write the contents to text file in C\#?**

Below is the sample code to write the contents to text file –

```text
Using System.IO;
File.WriteAllText(”mytextfilePath”, “MyTestContent”);
```

