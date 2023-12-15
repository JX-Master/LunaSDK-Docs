# Luna::includes

```c++
template <typename _InputIt1, typename _InputIt2, typename _Compare>
bool includes(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _Compare comp)
```

Checks if the sorted range [`first2`, `last2`) is a subsequence of the sorted range [`first1`, `last1`). (A subsequence need not be contiguous.) 



## Parameters
### first1
The iterator pointing to the first element of the first range. 

### last1
The iterator pointing to the one-past-last element of the first range. 

### first2
The iterator pointing to the first element of the second range. 

### last2
The iterator pointing to the one-past-last element of the second range. 

### comp
The user-provided binary predicate which returns `​true` if the first argument is less than the second. 

## Return value
Returns `true` if the sorted range [`first2`, `last2`) is a subsequence of the sorted range [`first1`, `last1`). Returns `false` otherwise. 

#### Valid Usage
* Elements in the ranges specified by [`first1`, `last1`) and [`first2`, `last2`) must be sorted in non-descending order.

* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of both `_InputIt1` and `_InputIt2`. 

