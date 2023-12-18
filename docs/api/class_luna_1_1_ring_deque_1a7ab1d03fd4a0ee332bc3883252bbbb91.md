# Luna::RingDeque::assign

```c++
template <typename _InputIter>
auto assign(_InputIter first, _InputIter last) -> enable_if_t<!is_integral_v< _InputIter >, void >
```

Replaces elements of the queue by elements specified by one range. Elements in the range will be copy-inserted into the queue. 



## Parameters
* *in* **first**

    The iterator to the first element of the range. 

* *in* **last**

    The iterator to the one-past-last element of the range. 

