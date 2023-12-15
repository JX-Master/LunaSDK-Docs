# Luna::ObjRef::attach

```c++
void attach(object_t ptr)
```

Attaches provided pointer. 

This call does not modify the reference counter of the new boxed object. The strong reference counter of the original boxed object, if not null, will be decreased before new pointer is attached. 

## Parameters
### ptr
The pointer to attach. 

