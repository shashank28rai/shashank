# Fibonacci series

public static void PrintFibonacciSeries\(int limit\) {

int digit1, digit2, digit3;

digit1 = 0;

digit2 = 1;

digit3 = digit1 + digit2;

Console.WriteLine\(digit1\);

Console.WriteLine\(digit2\);

Console.WriteLine\(digit3\);

for \(int i = 0; i &lt; limit; i++\) {

digit1 = digit2;

digit2 = digit3;

digit3 = digit1 + digit2;

Console.WriteLine\(digit3\);

}

}

## **Calling above method,**

static void Main\(string\[\] args\) {

clsFibonacci.PrintFibonacciSeries\(10\);

Console.ReadLine\(\);

}

## **Output:**

![ibonacci series](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/BlogImages/12172015122046PM/Fibonacci%20series.jpg)

