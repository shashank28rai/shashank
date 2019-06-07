# Factorial of number

public static int PrintFactorialOfNumber\(int number\)

{

// 7\*6

int result = 1;

for \(int i = number; i &gt; 0; i--\)

{

result = result \* i;

}

return result;

}

## **Calling above method:**

static void Main\( string \[\] args\)

{

int factorial;

factorial = clsfactorial.PrintFactorialOfNumber\(5\);

Console.WriteLine\("Factorial Of 5 Is " + factorial.ToString\(\)\);

```text
factorial = clsfactorial.PrintFactorialOfNumber\(7\);  

Console.WriteLine\("Factorial Of 7 Is " + factorial.ToString\(\)\);  

Console.ReadLine\(\);  
```

}

## **Output**

![Get Factorial of number](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/BlogImages/12172015122046PM/Get%20Factorial%20of%20number.jpg)

