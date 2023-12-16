# Luna::move_assign_range

```c++
template <typename _Iter1, typename _Iter2>
auto move_assign_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t<!Impl::move_assign_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Performs move assignment operation on every object in the destination range using the corresponding object in the source range. 



## Parameters
* *in* **first**

    An iterator to the first object to be moved from. 

* *in* **last**

    An iterator to one-past-last object to be moved from. 

* *in* **d_first**

    An iterator to the first object to be assigned. 

## Return value
Returns an iterator to the one-past-last object to be assigned. 

## Remark
The move operation is performed from first to last, the first element in destination range must not in the source range. `memmove` is used to move the data directly if:1. Both `_Iter1` and `_Iter2` are pointer types.

1. `value_type` of `_Iter1` and `_Iter2` is same.

1. `value_type` is trivially copy assignable and trivially move assignable. (If the type is trivially move assignable but not trivially copy assignable, the move assignment operator behaves the same as the copy assignment operator.) Otherwise, the move assignment operator is called for every object to move assign objects in destination range. 

