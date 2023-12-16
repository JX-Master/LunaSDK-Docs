# Luna::cast_object

```c++
template <typename _Rty>
_Rty * cast_object(object_t object_ptr)
```

Casts the object to the specified type. 



## Parameters
* *in* **object_ptr**

    The object pointer. 

## Return value
Returns `object_ptr` casted to the specified type if type casting is succeeded, returns `nullptr` otherwise. 

