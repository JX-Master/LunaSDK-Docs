# Luna::UniquePtr::UniquePtr

```c++
template <typename _D2, enable_if_t< negation_v< is_reference< _D2 > >, int >>
UniquePtr(pointer p, const deleter_type &d)
```

Constructs one smart pointer by wrapping pointer `p` with custom object deletion function. 



## Parameters
* **p**

    The pointer to wrap. 

* **d**

    The object deletion function used for the pointer. The function object will be copied into the smart pointer. 

