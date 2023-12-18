# Luna::set_difference

```c++
template <typename _InputIt1, typename _InputIt2, typename _OutputIt, typename _Compare>
_OutputIt set_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first, _Compare comp)
```

Copies elements that appear in the first sorted range and do not appear in the second sorted range to the destination range. The destination range is also sorted. 



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

* *in* **comp**

    The user-provided binary predicate which returns `​true` if the first argument is less than the second. 

## Return value
Returns one iterator to the one-past-last element of the destination range. 

## Remark
If [`first1`, `last1`) contains `m` elements that are equivalent to each other and [`first2`, `last2`) contains `n` elements that are equivalent to them, the final `max(m - n, 0)` elements will be copied from [`first1`, `last1`) to the output range, preserving order. 

## Valid Usage
* Elements in the ranges specified by [`first1`, `last1`) and [`first2`, `last2`) must be sorted in non-descending order.

* `comp` must have the following function signature: `bool comp(const Type& a, const Type& b)`, where `Type` is the value type of both `_InputIt1` and `_InputIt2`. 

