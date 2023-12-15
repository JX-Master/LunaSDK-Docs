# Luna::set_symmetric_difference

```c++
template <typename _InputIt1, typename _InputIt2, typename _OutputIt>
_OutputIt set_symmetric_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first)
```

Computes symmetric difference of two sorted ranges: elements that are found in either of the ranges, but not in both of them are copied to the destination range. The destination range is also sorted. 



## Parameters
### first1
The iterator pointing to the first element of the first range. 

### last1
The iterator pointing to the one-past-last element of the first range. 

### first2
The iterator pointing to the first element of the second range. 

### last2
The iterator pointing to the one-past-last element of the second range. 

### d_first
The iterator pointing to the first element of the destination range. 

## Return value
Returns one iterator pointing to the one-past-last element of the destination range. 

#### Valid Usage
* Elements in the ranges specified by [`first1`, `last1`) and [`first2`, `last2`) must be sorted in non-descending order. 

