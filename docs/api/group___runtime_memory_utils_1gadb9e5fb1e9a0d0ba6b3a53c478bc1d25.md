# Luna::default_construct_range

```c++
template <typename _Iter>
auto default_construct_range(_Iter first, _Iter last) -> enable_if_t< Impl::default_construct_range_is_value_type_class< _Iter >::value, void >
```

Default-constructs a range of objects. 



## Parameters
* *in* **first**

    An iterator to the first object to be constructed. 

* *in* **last**

    An iterator to one-past-last object to be constructed.


This function performs default initialization on each object in the range [`first`, `last`). 

## Remark
If _Ty is a class type (`is_class<_Ty>::value` is `true_type`), this function calls the default constructor for each object. Otherwise, this call does nothing, as described by C++ standard. ref: [https://en.cppreference.com/w/cpp/language/default_initialization](https://en.cppreference.com/w/cpp/language/default_initialization)

