# Luna::binary_search_iter

```c++
template <typename _ForwardIt, typename _Ty>
_ForwardIt binary_search_iter(_ForwardIt first, _ForwardIt last, const _Ty &value)
```

Finds an element equivalent to the specified value in the range. 



## Parameters
* *in* **first**

    The iterator to the first element of the range. 

* *in* **last**

    The iterator to the one-past-last element of the range. 

* *in* **value**

    The value to compare elements to. 

## Return value
Returns an iterator to the found element. If multiple equivalent elements exist in the range, returns the first one. Returns `last` if not found. 

## Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order. 

