# Difference Between Finalize and Dispose Method

.Net Framework provides two methods Finalize and Dispose for releasing unmanaged resources like files, database connections, COM etc.

| Dispose | Finalize |
| :--- | :--- |
| It is used to free unmanaged resources like files, database  connections etc. at any time | It can be used to free unmanaged resources \(when you         implement it\) like files, database connections etc. held by   an  object before that object is destroyed. |
| Explicitly, it is called by user code and the class which is       implementing dispose method, must has to implement        IDisposable interface. | Internally, it is called by Garbage Collector and cannot be      called by user code. |
| It belongs to IDisposable interface. | It belongs to Object class. |
| It's implemented by implementing IDisposable interface      Dispose\(\) method | It's implemented with the help of destructor in C++ & C\#. |
| There is no performance costs associated with Dispose     method. | There is performance costs associated with Finalize method since it doesn't clean the memory immediately and called by GC automatically. |
| This method uses interface – “IDisposable” interface and it will free up both managed and unmanaged codes like – database connection, files etc. | This method is called internally unlike Dispose method which is called explicitly. It is called by garbage collector and can’t be called from the code. |

