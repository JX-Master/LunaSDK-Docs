# Luna::binary_search_iter

```c++
template <typename _ForwardIt, typename _Ty, typename _Compare>
_ForwardIt binary_search_iter(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)
```

Finds an element equivalent to the specified value in the range. 



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
Returns an iterator pointing to the found element. If multiple equivalent elements exist in the range, returns the first one. Returns `last` if not found. 

#### Valid Usage
* Elements in the range specified by [`first`, `last`) must be sorted in non-descending order.

* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of `_ForwardIt`. 

