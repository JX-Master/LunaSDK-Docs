# Luna::copy_construct_range

```c++
template <typename _Iter1, typename _Iter2>
auto copy_construct_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t<!Impl::copy_construct_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Copy-constructs a range of objects. 



## Parameters
### first
An iterator to the first object to be copied from. 

### last
An iterator to one-past-last object to be copied from. 

### d_first
An iterator to the first object to be constructed. 

## Return value
Returns an iterator to the one-past-last object to be constructed.


This function uses each object in the range [`first`, `last`) to performs copy initialization on corresponding objects beginning with `d_first`. 

#### Valid Usage
* The source range and the destination range must not overlap. 

