# Luna::value_construct_range

```c++
template <typename _Iter>
auto value_construct_range(_Iter *first, _Iter *last) -> enable_if_t< Impl::value_construct_range_is_value_type_trivial< _Iter >::value, void >
```

Value-constructs a range of objects. 



## Parameters
* *in* **first**

    An iterator to the first object to be constructed. 

* *in* **last**

    An iterator to one-past-last object to be constructed.


This function performs value initialization on each object in the range [`first`, `last`). 

## Remark
This call uses `memzero` to clear all bytes in the storage to 0 if all of the following conditions are matched:1. `_Iter` is a pointer type.

1. `value_type` of `_Iter` is not a class type. Otherwise, this function calls the value constructor of each object. ref: [https://en.cppreference.com/w/cpp/language/value_initialization](https://en.cppreference.com/w/cpp/language/value_initialization)

