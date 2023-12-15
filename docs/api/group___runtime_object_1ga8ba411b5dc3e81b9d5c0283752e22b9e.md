# Luna::object_alloc

```c++
LUNA_RUNTIME_API object_t object_alloc(typeinfo_t type)
```

Allocates one boxed object. 

## Overview


## Parameters
### type
The type of the object to allocate. 

## Return value
Returns one pointer to the allocated object. The returned object is not initialized, the user should call constructors of the type manually. The returned object has 1 strong reference and 0 weak reference. 

