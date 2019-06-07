# C\# - Param Arrays

At times, while declaring a method, you are not sure of the number of arguments passed as a parameter. C\# param arrays \(or parameter arrays\) come into help at such times.

## The following example demonstrates this:

using System;  
namespace ArrayApplication  
{  
class ParamArray  
{  
public int AddElements\(params int\[\] arr\)  
{  
int sum = 0;  
foreach \(int i in arr\)  
{  
sum += i;  
}  
return sum;  
}  
}

class TestClass  
{  
static void Main\(string\[\] args\)  
{  
ParamArray app = new ParamArray\(\);  
int sum = app.AddElements\(512, 720, 250, 567, 889\);  
Console.WriteLine\("The sum is: {0}", sum\);  
Console.ReadKey\(\);  
}  
}  
}

When the above code is compiled and executed, it produces the following result:

The sum is: 2938

