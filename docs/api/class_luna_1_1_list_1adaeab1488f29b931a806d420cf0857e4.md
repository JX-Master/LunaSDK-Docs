# Luna::List::assign

```c++
template <typename _InputIt>
auto assign(_InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, void >
```

Replaces elements of the list by elements specified by one range. Elements in the range will be copy-inserted into the list. 



## Parameters
* *in* **first**

    The iterator to the first element of the range. 

* *in* **last**

    The iterator to the one-past-last element of the range. 

