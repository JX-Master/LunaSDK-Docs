# Luna::WeakRef::object

```c++
object_t object() const
```

Gets the boxed object. 

## Overview
This call does not modify the reference counter of the object. 

## Return value
Returns one pointer to the boxed object. Returns `nullptr` if the reference is null or the boxed object is expired. 

