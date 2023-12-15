# Luna::Ref::operator->

```c++
_Ty * operator->() const
```

Gets the boxed object casted to `_Ty`. 

This call does not modify the reference counter of the object. 

## Return value
Returns the interface or object pointer of the boxed object. Returns `nullptr` if the reference is not valid. 

