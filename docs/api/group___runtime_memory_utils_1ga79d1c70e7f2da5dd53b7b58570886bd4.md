# Luna::move_relocate_range_backward

```c++
template <typename _Iter1, typename _Iter2>
auto move_relocate_range_backward(_Iter1 first, _Iter1 last, _Iter2 d_last) -> enable_if_t< Impl::move_relocate_backward_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Relocates objects in the source range to a new range. 

This function behaves the same as [move_relocate_range](group___runtime_memory_utils_1ga63af54bbd0fa7737dc2d6b7a6d16e7fa.md), except that it relocates object from last to first, so the last object in the destination range should not in the source range. memmove is used instead of memcpy if the whole range can be relocated in one call. 

## Parameters
* *in* **first**

    An iterator to the first object to be relocated from. 

* *in* **last**

    An iterator to one-past-last object to be relocated from. 

* *in* **d_last**

    An iterator to the one-past-last object to be relocated to. 

## Return value
Returns an iterator to the front object to be relocated to in the destination range. 

