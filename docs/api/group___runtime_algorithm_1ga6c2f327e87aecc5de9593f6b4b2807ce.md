# Luna::set_intersection

```c++
template <typename _InputIt1, typename _InputIt2, typename _OutputIt>
_OutputIt set_intersection(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first)
```

Constructs a sorted range consisting of elements that are found in both sorted ranges. 



## Parameters
* *in* **first1**

    The iterator to the first element of the first range. 

* *in* **last1**

    The iterator to the one-past-last element of the first range. 

* *in* **first2**

    The iterator to the first element of the second range. 

* *in* **last2**

    The iterator to the one-past-last element of the second range. 

* *in* **d_first**

    The iterator to the first element of the destination range. 

## Return value
Returns one iterator to the one-past-last element of the destination range. 

## Remark
If [`first1`, `last1`) contains `m` elements that are equivalent to each otherand [`first2`, `last2`) contains `n` elements that are equivalent to them, the first `min(m, n)` elements will be copied from [`first1`, `last1`) to the output range, preserving order. 

## Valid Usage
* Elements in the ranges specified by [`first1`, `last1`) and [`first2`, `last2`) must be sorted in non-descending order. 

