# Luna::box_ptr

```c++
template <typename _Ty>
Ref< _Ty > box_ptr(_Ty *obj)
```

Creates a strong reference from one raw pointer without modifing its reference count. 



## Parameters
### obj
The raw pointer. 

## Return value
Returns the strong reference created from the raw pointer. 

