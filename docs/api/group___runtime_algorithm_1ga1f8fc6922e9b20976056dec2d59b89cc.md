# Luna::upper_bound

```c++
template <typename _ForwardIt, typename _Ty>
_ForwardIt upper_bound(_ForwardIt first, _ForwardIt last, const _Ty &value)
```

Finds the first element in the range such that `value < element` is `true`. 



## Parameters
* *in* **first**

    The iterator to the first element of the range. 

* *in* **last**

    The iterator to the one-past-last element of the range. 

* *in* **value**

    The value to compare elements to. 

## Return value
Returns an iterator to the first element in the range such that `value < element` is `true`, or `last` if no such element is found. 

## Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order. 

