# Luna::Ref::Ref

```c++
Ref(const Ref &rhs)
```

Constructs one reference by coping the pointer from another reference of the same type. 

The strong reference counter of the new boxed object, if not null, will be increased. 

## Parameters
* *in* **rhs**

    The reference to copy from. 

