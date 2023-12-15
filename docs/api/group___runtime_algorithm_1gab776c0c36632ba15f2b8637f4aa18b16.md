# Luna::includes

```c++
template <typename _InputIt1, typename _InputIt2>
bool includes(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2)
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

## Return value
Returns `true` if the sorted range [`first2`, `last2`) is a subsequence of the sorted range [`first1`, `last1`). Returns `false` otherwise. 

#### Valid Usage
* Elements in the ranges specified by [`first1`, `last1`) and [`first2`, `last2`) must be sorted in non-descending order. 

