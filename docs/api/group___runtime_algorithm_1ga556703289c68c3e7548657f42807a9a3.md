# Luna::set_symmetric_difference

```c++
template <typename _InputIt1, typename _InputIt2, typename _OutputIt, typename _Compare>
_OutputIt set_symmetric_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first, _Compare comp)
```

Computes symmetric difference of two sorted ranges: elements that are found in either of the ranges, but not in both of them are copied to the destination range. The destination range is also sorted. 



## Parameters
* *in* **first1**

    The iterator pointing to the first element of the first range. 

* *in* **last1**

    The iterator pointing to the one-past-last element of the first range. 

* *in* **first2**

    The iterator pointing to the first element of the second range. 

* *in* **last2**

    The iterator pointing to the one-past-last element of the second range. 

* *in* **d_first**

    The iterator pointing to the first element of the destination range. 

* *in* **comp**

    The user-provided binary predicate which returns `​true` if the first argument is less than the second. 

## Return value
Returns one iterator pointing to the one-past-last element of the destination range. 

## Remark
If [`first1`, `last1`) contains `m` elements that are equivalent to each otherand [`first2`, `last2`) contains `n` elements that are equivalent to them, then `abs(m - n)` of those elements will be copied to the output range, preserving order:* if `m > n`, the final `m - n` of these elements from [`first1`, `last1`).

* if `m < n`, the final `n - m` of these elements from [`first2`, `last2`). 

## Valid Usage
* Elements in the ranges specified by [`first1`, `last1`) and [`first2`, `last2`) must be sorted in non-descending order.

* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of both `_InputIt1` and `_InputIt2`. 

