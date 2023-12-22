# lustruct

```c++
#define lustruct(_name, _guid)
```

Declares the name and guid for one structure or class type. 



## Parameters
* *in* **name**

    The name string of the type. 

* *in* **guid**

    The GUID string of the type. 

## Remark
Add this macro to the type body. For exmaple: ``` struct MyType { lustruct("MyType", "{dbeecd7a-2dc5-423e-8e20-7521826c3f06}"); // other members... }; 

