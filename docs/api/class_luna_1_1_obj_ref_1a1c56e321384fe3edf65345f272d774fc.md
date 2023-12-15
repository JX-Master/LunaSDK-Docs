# Luna::ObjRef::get

```c++
object_t get() const
```

Gets the boxed object. 

This call does not modify the reference counter of the object. 

## Return value
Returns one pointer to the boxed object. Returns `nullptr` if the reference is null. 

