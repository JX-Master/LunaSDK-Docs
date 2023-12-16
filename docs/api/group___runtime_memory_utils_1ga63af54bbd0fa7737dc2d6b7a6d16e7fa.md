# Luna::move_relocate_range

```c++
template <typename _Iter1, typename _Iter2>
auto move_relocate_range(_Iter1 first, _Iter1 last, _Iter2 d_first) -> enable_if_t< Impl::move_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Relocates objects in the source range to a new range. 

This function behaves the same as [copy_relocate_range](group___runtime_memory_utils_1gab176a0253de8e05b3ff0c9d5c3bb0f04.md), except that it allows the destination range overlaps with the source range, proved that the first object in the destination range does not in the source range. memmove is used instead of memcpy if the whole range can be relocated in one call. 

## Parameters
* *in* **first**

    An iterator to the first object to be relocated from. 

* *in* **last**

    An iterator to one-past-last object to be relocated from. 

* *in* **d_first**

    An iterator to the first object to be relocated to. 

## Return value
Returns an iterator to the one-past-last object to be relocated to. 

