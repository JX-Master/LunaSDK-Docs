# Luna::copy_construct_range_n

```c++
template <typename _Iter1, typename _Iter2>
auto copy_construct_range_n(_Iter1 first, usize count, _Iter2 d_first) -> enable_if_t<!Impl::copy_construct_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Copy-constructs a range of objects. The range is provided by first object and object count. 



## Parameters
* *in* **first**

    An iterator to the first object to be copied from. 

* *in* **count**

    The number of objects to copy-construct. 

* *in* **d_first**

    An iterator to the first object to be constructed. 

## Return value
Returns an iterator to the one-past-last object to be constructed.


This function uses each object in the range [`first`, `first + count`) to performs copy initialization on corresponding objects beginning with `d_first`. 

## Valid Usage
* The source range and the destination range must not overlap. 

## Remark
`memcpy` is used to copy the data directly if:1. Both `_Iter1` and `_Iter2` are pointer types.

1. `value_type` of `_Iter1` and `_Iter2` is same.

1. `value_type` is trivially copy constructible. Otherwise, the copy constructor is called for every object to construct objects in destination range. 

