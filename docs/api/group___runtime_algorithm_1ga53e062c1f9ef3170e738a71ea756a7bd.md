# Luna::equal_range

```c++
template <typename _ForwardIt, typename _Ty>
Pair< _ForwardIt, _ForwardIt > equal_range(_ForwardIt first, _ForwardIt last, const _Ty &value)
```

Gets a range containing all elements equivalent to the specified value in the range. 



## Parameters
* *in* **first**

    The iterator to the first element of the range. 

* *in* **last**

    The iterator to the one-past-last element of the range. 

* *in* **value**

    The value to compare elements to. 

## Return value
Returns a pair of iterators pointing to the begin and end of the range. The first iterator points to the first element of the range, the second iterator points to the one-past-last element of the range. If the specified element is not found in the range, returns one pair of iterators that are equal to each other. 

## Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order. 

