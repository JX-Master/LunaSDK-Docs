# Luna::Ref::operator=

```c++
Ref & operator=(_Ty *ptr)
```

Assigns this reference using the native pointer of the same type. 

The strong reference counter of the new boxed object, if not null, will be increased. The strong reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### ptr
The native pointer to set. 

