# Luna::UniquePtr::reset

```c++
void reset(pointer ptr=pointer())
```

Sets the native pointer of this smart pointer. If this smart pointer is not null, the original instance pointed by this smart pointer will be deleted. 



## Parameters
* *in* **ptr**

    The new pointer to set. If this is not provided, the smart pointer will be cleared to null. 

