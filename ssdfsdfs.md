# Differences Between Structures and Classes

1. **Structures** are value types ,use stack memory and the **classes** are reference types, use heap memory.
2. **Classes** are usually used for large amounts of data, whereas  **structs** are usually used for smaller amounts of data.
3. **Classes** can be inherited whereas **structures** not.
4. A **structure** couldn't be null like a class.
5. A **structure** couldn't have a destructor such as a class.
6. A **structure** can't be abstract, a class can.
7. A **class** has all members private by default. A **struct** is a class   where members are public by default.
8. **Class** can have constructor and destructor of all types and **Structure** can only have the parametrized constructor. it means a **structure** can not have the non-parametrized constructor,default constructor and destructor also.
9. The member variable can be initialized directly in **class** and The member variable cannot be initialized directly in **structure**.
10. **Class** object cannot be created without using the new keyword, it means we have to use it. Eg: Demo obj=new Demo\(\) and **Structure** object can be created without using the new keyword.\(optional\). Eg: Demo obj;

