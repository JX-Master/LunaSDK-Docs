# Luna::copy_assign_range

```c++
template <typename _Iter1, typename _Iter2>
auto copy_assign_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t<!Impl::copy_assign_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Performs copy assignment operation on every object in the destination range using the corresponding object in the source range. 



## Parameters
* *in* **first**

    An iterator to the first object to be copied from. 

* *in* **last**

    An iterator to one-past-last object to be copied from. 

* *in* **d_first**

    An iterator to the first object to be assigned. 

## Return value
Returns an iterator to the one-past-last object to be assigned. 

## Valid Usage
* The source range and the destination range must not overlap. 

## Remark
`memcpy` is used to copy the data directly if:1. Both `_Iter1` and `_Iter2` are pointer types.

1. `value_type` of `_Iter1` and `_Iter2` is same.

1. `value_type` is trivially copy assignable. Otherwise, the copy assignment operator is called for every object to copy assign objects in destination range. 

