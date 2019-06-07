# How Assembly can Improve Application Performance

CLR is place where .Net Application codes gets compiled. Whenever you made an request to ASP.NET page, the page gets compiled first and then is transferred to the user. The compilation process is also completed in two steps.

* 1. An IL \(**Intermediate Language**\) is generated and then this is handed over for JIT
* 1. JIT \(**Just In Time**\) compilation which produces the machine code and our pages get displayed with their dynamic content.

The performance of our web application can be improved by creating pre-compiled libraries of IL which can then be handed over to JIT directly without having the inclusion of an extra process to make the conversion. This method is calledcomponentization. Components are pre-compiled set of classes that have been developed in the form of**DLL**files and can then be included within our projects. This is also known as an assembly.

