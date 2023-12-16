# Luna::binary_search

```c++
template <typename _ForwardIt, typename _Ty>
bool binary_search(_ForwardIt first, _ForwardIt last, const _Ty &value)
```

Checks if an element equivalent to the specified value appears within the range. 



## Parameters
* *in* **first**

    The iterator pointing to the first element of the range. 

* *in* **last**

    The iterator pointing to the one-past-last element of the range. 

* *in* **value**

    The value to compare elements to. 

## Return value
Returns `true` if an element equal to `value` is found, `false` otherwise. 

## Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order. 

