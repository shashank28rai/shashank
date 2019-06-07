# Types of Assemblies in .Net

## Types of Assemblies in .Net:-

* Private and Shared Assemblies
* Static and Dynamic Assemblies
* Single-File and Multifile Assemblies
* Satellite and Resource-only Assemblies

## Private Assembly

* When you deploy an assembly which can be use by single application, than this assembly is called a **private assembly.**
* **Private assemblies** can be used by only one application they are deployed with.
* **Private assemblies** are deployed in the directory where the main application is installed.

## Shared Assembly

* When you deploy an assembly which can be used by several application, than this assembly is called **shared assembly**.
* **Shared assemblies** are stored in a special folder called Global Assembly Cache \(GAC\), which is accessible by all applications.
* **Shared assemblies** must have a strong name. A strong name consists of an assembly name, a version number, a culture, a public key and an optional digital signature.
* GAC is capable of maintaining multiple copies of an assembly with the same name but different versions.

## Static Assembly

A static assembly is created when you compile the program using any of the .NET language compilers. A static assembly

contains the types, interfaces, and various resources required by the assembly. A static assembly is stored on the hard disk in the form of a portable executable \(.exe or .dll\) file. In a simple term, when you compile through VS.Net it generates files which are physically stored on the disk, this files are called static assembly.

## Dynamic Assembly

Assemblies which are created and execute on the fly are called dynamic assembly. You can create dynamic assembly through System.Reflection.Emit namespace.

## Single-File Assembly

A single-file assembly consists of a single .exe or .dll file.

### [Example of Single File Assembly](http://dotnetguts.blogspot.com/2007/09/creating-component-in-net.html)

In the example the Shape.dll generated is a Single File Assembly.

## Multifile Assembly

* A multifile assembly is an assembly that can include multiple file, but it should contain atleast one .dll or .exe file.
* Assembly manifest in multifile assembly can be attached to any assembly file or can be created seperately just the manifest.

## Satellite Assembly

Resource-only assemblies are assembly's that stores only resource and no code. example, Image. Resource-only assemblies that store the culture-specific information are known as satellite assemblies.

