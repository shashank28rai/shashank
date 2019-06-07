# Why multiple inheritance is not possible on c\#.net

```text
 Class Shape1{

 public void CalculateArea()
 {  }
 }
//There is another class shape2 that one also has same method
Class Shape2{

public void CalculateArea() {  }

}
//Now i have a child class Circle, it derives from both SHape1 and shape2;
public class Circle: Shape1,shape2
{
}
```

* Now when i create object for Circle, and call the method, system doesn't know which calculate area method to be called.
* Both has same signatures. So compiler will get confuse .that's why multiple inheritances are not allowed.
* But there can be multiple interfaces because interfaces dont ve method definition.
* Even both the interfaces have same method, both of them dont ve any implementation and always method in the child class will be executed.

