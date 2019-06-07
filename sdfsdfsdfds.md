# Difference Between Constant and Read Only and Static

## **Constant:-**

Constant fields or local variables must be assigned a value at the time of declaration and after that they cannot be modified. By default constant are static, hence you cannot define a constant type as static.

1. public constant X =10;

A const field is a compile-time constant. A constant field or local variable can be initialized with a constant expression which must be fully evaluated at compile time.

1. void Calculate\(intZ\){
2. constant X =10, X1 =50;
3. constant Y = X + X1;//no error, since its evaluated a compile time
4. constant Y1 = X + Z;//gives error, since its evaluated at run time
5. }

You can apply const keyword to built-in value types \(byte, short, int, long, char, float, double, decimal, bool\), enum, a string literal, or a reference type which can be assigned with a value null.

1. const MyClassobj1 = null;//no error, since its evaluated a compile time
2. const MyClassobj2 =newMyClass\(\);//gives error, since its evaluated at run time

Constants can be marked as public, private, protected, internal, or protected internal access modifiers.

Use the const modifier when you sure that the value a field or local variable would not be changed.

## **ReadOnly :-**

A readonly field can be initialized either at the time of declaration or with in the constructor of same class. Therefore, readonly fields can be used for run-time constants.

1. class MyClass {
2. readonly intX =10;// initialized at the time of declaration
3. readonly intX1;
4. public MyClass\(intx1\){
5. X1 = x1;// initialized at run time
6. }
7. }

Explicitly, you can specify a readonly field as static since, like constant by default it is not static. Readonly keyword can be apply to value type and reference type \(which initialized by using the new keyword\) both. Also, delegate and event could not be read only.

## **Static :-**

The static keyword is used to specify a static member, which means static members are common to all the objects and they do not tied to a specific object. This keyword can be used with classes, fields, methods, properties, operators, events, and constructors, but it cannot be used with indexers, destructors, or types other than classes.

1. class MyClass{
2. static intX =10;
3. intY =20;
4. public staticvoidShow\(\){
5. Console.WriteLine\(X\);
6. Console.WriteLine\(Y\);//error, since you can access only static members
7. }
8. }

