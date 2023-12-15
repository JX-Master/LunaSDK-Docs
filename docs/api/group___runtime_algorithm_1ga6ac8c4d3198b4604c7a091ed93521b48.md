# Luna::lower_bound

```c++
template <typename _ForwardIt, typename _Ty, typename _Compare>
_ForwardIt lower_bound(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)
```

Finds the first element in the range such that `comp(element, value)` is `false`. 

## Overview


## Parameters
### first
The iterator pointing to the first element of the range. 

### last
The iterator pointing to the one-past-last element of the range. 

### value
The value to compare elements to. 

### comp
The user-provided binary predicate which returns `​true` if the first argument is less than the second. 

## Return value
Returns an iterator pointing to the first element in the range such that `comp(element, value)` is `false`, or `last` if no such element is found. 

#### Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order.

* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of `_ForwardIt`. 
