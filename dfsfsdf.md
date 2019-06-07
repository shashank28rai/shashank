# Difference between namespace and assembly

## **Assembly:**

An assembly provides a fundamental unit of physical code grouping.It is an Output Unit. It is a unit of Deployment & a unit of versioning. Assemblies contain MSIL code.

## **Namespace:**

A namespace provides a fundamental unit of logical code grouping.It is a Collection of names wherein each name is Unique.They form the logical boundary for a Group of classes.Namespace must be specified in Project-Properties.

| **Namespace** | **Assembly** |
| :--- | :--- |
| Namespace is the logical naming decided at design time by the developer. | Scope for a particular type is defined at run time using         Assembly. |
| Namespace contains set of unique names. | Assembly contains code of the form MSIL \( Microsoft Intermediate Language\) |
| Classes available in your program will be logically grouped   together under a namespace. | Logical units are physically grouped together as assembly. |
| Namespace can include multiple assemblies. | An assembly can contain types belonging to different namespaces. |
| Namespace doesn't have any classification. | Assembly can be classified as private assembly and public assembly. Private assembly is specific to a single application but shared/public assembly contains libraries which can be used by multiple applications. |
| Namespaces have to be mentioned in Project-Properties. | Assemblies need not be explicitly specified. They are automatically described in metadata and manifest files. |
| Namespaces can be nested. For example: namespace sampleApp1 { namespace SampleApp2 { class sampleClass { … } } } | Such nesting is not permissible in assemblies. |
| Namespace is the one which you directly specify in your code. A simple example for namespace is shown below: namespace sampleNamespace { class sampleClass { public void displayMsg\(\) { Console.WriteLine\("In sampleClass"\); } } } In this example, sampleNamespace is the namespace you have created and sampleClass is within the scope of this namespace. | Creating an assembly on your own is not as simple as you create a namespace. If you want to package the code shown as an example for the namespace into an assembly, then you have to follow the steps shown below: " Generate a key file inside the same folder where you have placed the code by typing the following statement in the command prompt: sn -k sampleKey.key " Sign your code component with this key. Assume that your code component is named as sampleClass.cs. Now use the following command: csc sampleClass.cs /t:library /a.keyfile:sampleKey.key " Place your signed assembly inside GAC using AL Utility: AL /i: sampleClass.dll " Now create a code that accesses the code in your assembly: Using System; Using sampleNamespace; public class testClass { sampleClass obj = new sampleClass\(\); obj.displayMsg\(\); } " To test if your assembly got created and to test if the above code is working, compile the above code using the following statement: csc testClass.cs /t:exe /r:&lt;path of your assembly&gt; " Now if you execute testClass.cs, you should get the following output: In sampleClass |

