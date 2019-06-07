# What is "DLL Hell" Problem

* **DLL Hell** problem occurs due to version incompatibility of dll's.
* **DLL HELL** is the problem that occures when an installation of a newer application might break or hinder other application as newer DLLs are copied into the system and the older application do not support or not compatible with them. .net overcomes this problem by supporting multiple versions of an assembly at any given time.this is called side-by-side component versioning More on "**DLL Hell**" Problem.
* **DLL Hell** is a problem occurs when multiple applications attempt to share a common component like a dynamic link library \(DLL\) or a Component Object Model \(COM\) class.
* In the most typical case, one application will install a new version of the shared component that is not backward compatible with the version already on the machine. 
* Although the application that has just been installed works well, existing applications that depended on a previous version of the shared component might no longer work.

