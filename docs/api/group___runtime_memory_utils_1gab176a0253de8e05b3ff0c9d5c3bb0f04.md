# Luna::copy_relocate_range

```c++
template <typename _Iter1, typename _Iter2>
auto copy_relocate_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::copy_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Relocates objects in the source range to a new range that is not overlap with the source range. 

After this call, the objects in the destination range behaves the same as the corresponding objects formerly in the source range, except that the places(memory addresses) for objects are changed. 

## Parameters
* *in* **first**

    An iterator to the first object to be relocated from. 

* *in* **last**

    An iterator to one-past-last object to be relocated from. 

* *in* **d_first**

    An iterator to the first object to be relocated to. 

## Return value
Returns an iterator to the one-past-last object to be relocated to. 

## Valid Usage
* The iterator for the source range and destination range must have the same `value_type`. 

## Remark
All objects in the destination range must in uninitialized state before this call. And after this call, all objects in the source range is in uninitialized state.


This call behaves differently in the following different conditions:

1. If `value_type` of `_Iter1` is trivially relocatable (which is always true unless the user explicitly demonstrates), `memcpy` is used to copy the data from source place to destination place. If `_Iter` and `_Iter2` is both pointer types, the full range will be copied by `memcpy` in one call, otherwise, `memcpy` will be called once per object. No constructors and destructors are called in this period.

1. If `value_type` of `_Iter1` is not trivially relocatable, for every object in the destination range, the move constructor will be called with the corresponding object in the source range passed in, then the destructor of the corresponding object in the source range will be called. 

