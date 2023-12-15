# Luna::default_construct_range

```c++
template <typename _Iter>
auto default_construct_range(_Iter first, _Iter last) -> enable_if_t< Impl::default_construct_range_is_value_type_class< _Iter >::value, void >
```

Default-constructs a range of objects. 

## Overview


## Parameters
### first
An iterator to the first object to be constructed. 

### last
An iterator to one-past-last object to be constructed.


This function performs default initialization on each object in the range [`first`, `last`). 

