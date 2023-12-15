# Luna::equal_range

```c++
template <typename _ForwardIt, typename _Ty, typename _Compare>
Pair< _ForwardIt, _ForwardIt > equal_range(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)
```

Gets a range containing all elements equivalent to the specified value in the range. 

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
Returns a pair of iterators pointing to the begin and end of the range. The first iterator points to the first element of the range, the second iterator points to the one-past-last element of the range. If the specified element is not found in the range, returns one pair of iterators that are equal to each other. 

#### Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order.

* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of `_ForwardIt`. 

