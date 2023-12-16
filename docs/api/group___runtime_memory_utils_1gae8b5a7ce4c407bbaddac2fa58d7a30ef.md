# Luna::memzero

```c++
template <typename _Ty>
_Ty * memzero(_Ty *dst)
```

Clears the memory of the specified object to 0. 



## Parameters
* *in* **dst**

    The object to clear. The size of the memory region to clear will be `sizeof(_Ty)`. 

## Return value
Returns the `dst` pointer. 

