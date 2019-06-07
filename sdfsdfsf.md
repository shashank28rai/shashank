# Difference between string and String builder

**String:-** 

* String is an immutable object ones object is crated then It can not be modified .
* If there is any changes then create new object. string object is used to concatenating two string like String str=”Hi”; Str+=”Ho r u?”;.
* Immutable like when we create string object in code so we cannot modify or change that object in any operations like insert new value, replace or append any value with existing value in string object
* When we have to do some operations to change string simply it will dispose the old value of string object and it will create new instance in memory for hold the new value in string object like:

![ASP.NET](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/8ef97c/C-Sharp-net-interview-questions-and-answers/Images/image008.png)  
**Note:**

* It’s an immutable object that hold string value.
* Performance wise string is slow because its’ create a new instance to override or change the previous value.
* String belongs to System namespace.

**StringBuilder:** 

 ****If we create string builder the we can perform action like insert ,replace ,append without crated new instance.    
****System.Text.Stringbuilder is mutable object which also hold the string value, mutable means once we create a System.Text.Stringbuilder object we can use this object for any operation like insert value in existing string with insert functions also replace or append without creating new instance of System.Text.Stringbuilder for every time so it’s use the previous object so it’s work fast as compare than System.String. Let’s have an example to understand System.Text.Stringbuilder like:

![ASP.NET](http://csharpcorner.mindcrackerinc.netdna-cdn.com/UploadFile/8ef97c/C-Sharp-net-interview-questions-and-answers/Images/image009.png)  
**Note:**

* StringBuilder is a mutable object.
* Performance wise StringBuilder is very fast because it will use same instance of StringBuilder object to perform any operation like insert value in existing string.
* StringBuilder belongs to System.Text.Stringbuilder namespace.

