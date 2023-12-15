# Luna::Ref::object

```c++
object_t object() const
```

Gets the boxed object. 

This call does not modify the reference counter of the object. 

## Return value
Returns one pointer to the boxed object. Returns `nullptr` if the reference is null. 

