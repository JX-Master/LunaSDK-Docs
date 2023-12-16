# Luna::move_assign_range_backward

```c++
template <typename _Iter1, typename _Iter2>
auto move_assign_range_backward(_Iter1 first, _Iter1 last, _Iter2 d_last) -> enable_if_t<!Impl::move_assign_range_backward_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter2 >
```

Same as [move_assign_range](group___runtime_memory_utils_1ga2922440bc8a0efbe2c479e0b9d710a91.md), but performs the move assign from back to front. 



## Parameters
* *in* **first**

    An iterator to the first object to be moved from. 

* *in* **last**

    An iterator to one-past-last object to be moved from. 

* *in* **d_last**

    An iterator to the one-past-back object in the range to be assigned. 

## Return value
Returns an iterator to the front object in the range to be assigned.


The last element in destination range must not in the source range. 

