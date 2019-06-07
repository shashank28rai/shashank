# Exchange Two integer variable value without using third variable

public static void ExchangeInteger\(\)

{

int a = 10;

int b = 5;

Console.WriteLine\("a={0}", a\);

Console.WriteLine\("b={0}", b\);

a = a + b;

// Now a would be 15

b = a - b;

// Now b would be 15-5=10 ........

a = a - b;

// Now a would be 15-10=5........

Console.WriteLine\("a={0}", a\);

Console.WriteLine\("b={0}", b\);

Console.ReadLine\(\);

}

## **Calling above method,**

1. static void  Main\(string\[\] args\)  
2. {  
3. clsExchangevariable.ExchangeInteger\(\);  
4. }  

## **Output**

![Exchange Two integer variable value](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/BlogImages/12172015122046PM/Exchange%20Two%20integer%20variable%20value.jpg)

