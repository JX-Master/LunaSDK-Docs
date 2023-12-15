# Luna::move_construct_range

```c++
template <typename _Iter1, typename _Iter2>
auto move_construct_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::move_construct_range_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Move-constructs a range of objects. 



## Parameters
### first
An iterator to the first object to be moved from. 

### last
An iterator to one-past-last object to be moved from. 

### d_first
An iterator to the first object to be constructed. 

## Return value
Returns an iterator to the one-past-last object to be constructed.


This function uses each object in the range [`first`, `last`) to performs move initialization on corresponding objects beginning with `d_first`. 

#### Valid Usage
* The source range and the destination range must not overlap. 

