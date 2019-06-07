# C\# Static

* C\# includes "**static**" keyword just like other programming languages such as C++, Java, etc. 
* The **Static** keyword can be applied on classes, variables, methods, properties, operators, events and constructors. 
* However, it cannot be used with indexers, destructors or types other than classes.
* The **Static** modifier makes an item non-instantiable, it means the static item cannot be instantiated. 
* If the **static** modifier is applied to a class then that class cannot be instantiated using the **new** keyword. 
* If the **static** modifier is applied to a variable, method or property of class then they can be accessed without creating an object of the class, just use className.propertyName, className.method Name.

## Example:-

\`\`\`C \#  
public static class MyStaticClass  
{  
public static int myStaticVariable = 0;

public static void MyStaticMethod\(\)

```text
{
```

Console .WriteLine\("This is a static method."\);  
}

public static int MyStaticProperty { get; set; }  
}

class Program  
{

static void Main\(string\[\] args\)  
{

Console.WriteLine\(MyStaticClass.myStaticVariable\);

MyStaticClass .MyStaticMethod\(\);

```text
    MyStaticClass.MyStaticProperty = 100;
```

Console.WriteLine\(MyStaticClass.MyStaticProperty\);  
}  
}

## Output:

0

This is a static method.

100

In the above example, MyStaticClass is a static class with static variable, method and property. All the static members can be access using className without creating an object of a class e.g. MyStaticClass.MyStaticMethod\(\).

Static method can only access other static items.It is also possible to have static members in non-static classes just like a normal class. You can instantiate non static classes using the new keyword as usual. However, the instance variable can only access the non-static methods and variables, it cannot access the static methods and variables.

## For example, consider the following myNonStaticClass with mix of static and non-static methods:

## Example: Static members in non-static class

```text
public class MyNonStaticClass
{    
private static int  myStaticVariable = 0;    
public static void  MyStaticMethod()
    {
        Console.WriteLine("This is static method.");
    }


public void  myNonStaticMethod()
    {
        Console.WriteLine("Non-static method");
    }
}
```

In the above example, MyNonStaticClass can be instantiated and access the non-static members. However, you cannot access static members. The following figure shows the debug view.

[![Non-Static method](http://www.tutorialsteacher.com/Content/images/csharp/nonstatic-method.png)](http://www.tutorialsteacher.com/Content/images/csharp/nonstatic-method.png)

Non-Static method

