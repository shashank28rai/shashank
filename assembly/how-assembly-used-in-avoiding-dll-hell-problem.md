# How Assembly used in Avoiding "DLL Hell" Problem

* "**DLL Hell**" Problem is solved in .Net using Assembly.Each assembly has a version number. 
* All the types and resources in an assembly share the same version number to make it easy for applications to refer to the correct version of files and avoid problem of "**DLL Hell**". Thus assemblies allows the execution of multiple versions of the same assembly on the same machine.
* The side-by-side execution of assemblies overcomes the problem known as "**DLL hell**" which is one of the major problems associated with COM applications.

