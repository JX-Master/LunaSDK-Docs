# Luna::equal

```c++
template <typename _Iter1, typename _Iter2, typename _EqualComp>
bool equal(_Iter1 first1, _Iter1 last1, _Iter2 first2, _EqualComp equal_compare)
```

Tests the equality of two ranges. 



## Parameters
### first1
The iterator pointing to the first element of the first range. 

### last1
The iterator pointing to the one-past-last element of the first range. 

### first2
The iterator pointing to the first element of the second range. 

### equal_compare
The user-defined equal (==) comparison function used for comparing. 

## Return value
Returns `true` if two ranges are equal, returns `false` otherwise. 

