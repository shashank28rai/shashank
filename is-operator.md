# is Operator and as Operator

## **is Operator and as Operator :-**

The "**is**" operator is used to check whether the run-time type of an object is compatible with a given type or not. In other words, we use the "**is**" operator to verify that the type of an object is what we expect it to be. Let's look at its syntax:

expression is type

### Example of the "is" operator:

usingSystem;  
classClass1  
{ }  
classClass2  
{ }  
public classIsTest  
{  
public static void Test\(object o\)  
{  
Class1 a;  
Class2 b;  
if\(o is Class1\)  
{  
Console.WriteLine\("o is Class1"\);  
a = \(Class1\)o;  
}  
elseif\(o is Class2\)  
{  
Console.WriteLine\("o is Class2"\);  
b = \(Class2\)o;  
}  
else  
{  
Console.WriteLine\("o is neither Class1 nor Class2."\);  
}  
}  
publicstaticvoidMain\(\)  
{  
Class1 c1 =new Class1\(\);  
Class2 c2 =new Class2\(\);  
Test\(c1\);  
Test\(c2\);  
Test\("Passing String Value instead of class"\);  
Console.ReadKey\(\);  
}  
}

![image001.png](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/abhikumarvatsa/the-is-and-as-operators-in-C-Sharp/Images/image001.png)

In the above example, I'll be checking whether object o is a class or not. If the argument passed is not a class then the application will jump to the message 'o is neither class1 nor class2'.

## **as Operator**

The "**as**" operator is used to perform conversions between compatible types. Actually, the "**as**" operator fulfills a similar role like "**is**" but in a slightly truncated manner. Let's look at its syntax:

expression as type

Example of the "is" operator:

usingSystem;  
classClass1  
{  
}  
classClass2  
{  
}  
publicclassIsTest  
{  
public static void Main\(\)  
{  
object\[\] myObjects =new object\[6\];  
myObjects\[0\] =new Class1\(\);  
myObjects\[1\] =new Class2\(\);  
myObjects\[2\] ="string";  
myObjects\[3\] = 32;  
myObjects\[4\] =null;  
for\(inti = 0; i &lt; myObjects.Length; ++i\)  
{  
strings = myObjects\[i\] as string;  
Console.Write\("{0}:", i\);  
if\(s !=null\)  
Console.WriteLine\("'"+ s +"'"\);  
else  
Console.WriteLine\("not a string"\);  
}  
Console.ReadKey\(\);  
}  
}

![image002.png](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/abhikumarvatsa/the-is-and-as-operators-in-C-Sharp/Images/image002.png)

In the above example, each and every value is being cast to a string using the "**as**" operator and assigned to a string variable which is shown on the console.

So, that's all about the "**is**" and "**as**" operators.

