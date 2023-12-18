# Luna::equal

```c++
template <typename _Iter1, typename _Iter2, typename _EqualComp>
bool equal(_Iter1 first1, _Iter1 last1, _Iter2 first2, _EqualComp equal_compare)
```

Tests the equality of two ranges. 



## Parameters
* *in* **first1**

    The iterator to the first element of the first range. 

* *in* **last1**

    The iterator to the one-past-last element of the first range. 

* *in* **first2**

    The iterator to the first element of the second range. 

* *in* **equal_compare**

    The user-defined equal (==) comparison function used for comparing. 

## Return value
Returns `true` if two ranges are equal, returns `false` otherwise. 

