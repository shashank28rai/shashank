# Copy Constructor

## Example for Copy Constructor:-

using System;

namespace ProgramCall  
{  
classTest2  
{  
int A, B;  
public Test2\(int X, int Y\)  
{  
A = X;  
B = Y;  
}

//Copy Constructor  
public Test2\(Test2 T\)  
{  
A = T.A;  
B = T.B;  
}

public void Print\(\)  
{  
Console.WriteLine\("A = {0}\tB = {1}", A, B\);  
}

}

classCopyConstructor  
{  
staticvoid Main\(\)  
{

Test2 T2 = newTest2\(80, 90\);  
//Invoking copy constructor  
Test2 T3 = newTest2\(T2\);  
T2.Print\(\);  
T3.Print\(\);  
Console.Read\(\);  
}  
}  
}

Output

A = 80 B = 90  
A = 80 B = 90

