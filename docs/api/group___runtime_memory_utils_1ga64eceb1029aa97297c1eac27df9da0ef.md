# Luna::destruct_range

```c++
template <typename _Iter>
auto destruct_range(_Iter first, _Iter last) -> enable_if_t< Impl::destruct_range_is_value_type_trivial< _Iter >::value, void >
```

Destructs every object in the range. 



## Parameters
### first
An iterator to the first object to be destructed. 

### last
An iterator to one-past-last object to be destructed. 

