# What is Assembly

* An **assembly** is a file that is automatically generated by the compiler upon successful compilation of every .NET application. 
* It can be either a Dynamic Link Library or an executable file.
* It is generated only once for an application and upon each subsequent compilation the assembly gets updated.
* When a source code is compiled by the language compiler it Generate a Managed Assembly and MSIL\(MisroSoft Intermediate Language\). That Assembly contains .dll or .exe file. 
* An **Assebmly** can be of two types Private Assembly and Shared Assembly, shared Assembly is stored in GAC\(Global Assembly Cache\) so that any application can refer to it while private assembly is stored in application folder which can be used by only one Application.

Assembly is a logical collection of smallest unit in .Net Framework.

* Example: .DLL File contains the application code, the .aspx file, .ascx user controls, .gif, .bmp, .ico file and other files like Resource file \(.resx\), etc.
* In summary, Assemblies is a basic fundamental unit of application development and deployment in the .Net Framework
* An assembly contains the MSIL code, which the common language runtime executes, and the type metadata.
* An assembly also contains an assembly manifest that contains the assembly metadata. This metadata contains information about the assembly version, its security identity, the resources required by the assembly, and the scope of the assembly.
* Assemblies are the smallest units to which the .NET Framework grants permissions. They provide security boundaries within the .NET Framework. You specify the permission required by your application while building assemblies. When the assembly is loaded into the runtime, the assembly sends a request to the runtime to grant the permission.

