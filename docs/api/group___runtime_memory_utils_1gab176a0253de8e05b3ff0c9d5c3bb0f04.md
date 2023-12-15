# Luna::copy_relocate_range

```c++
template <typename _Iter1, typename _Iter2>
auto copy_relocate_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::copy_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Relocates objects in the source range to a new range that is not overlap with the source range. 

After this call, the objects in the destination range behaves the same as the corresponding objects formerly in the source range, except that the places(memory addresses) for objects are changed. 

## Parameters
### first
An iterator to the first object to be relocated from. 

### last
An iterator to one-past-last object to be relocated from. 

### d_first
An iterator to the first object to be relocated to. 

## Return value
Returns an iterator to the one-past-last object to be relocated to. 

#### Valid Usage
* The iterator for the source range and destination range must have the same `value_type`. 


This call behaves differently in the following different conditions:

