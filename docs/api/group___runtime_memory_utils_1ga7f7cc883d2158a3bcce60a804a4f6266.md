# Luna::value_construct_range

```c++
template <typename _Iter>
auto value_construct_range(_Iter *first, _Iter *last) -> enable_if_t< Impl::value_construct_range_is_value_type_trivial< _Iter >::value, void >
```

Value-constructs a range of objects. 



## Parameters
### first
An iterator to the first object to be constructed. 

### last
An iterator to one-past-last object to be constructed.


This function performs value initialization on each object in the range [`first`, `last`). 

