# Luna::max

```c++
template <typename _Ty, typename _LessComp>
constexpr const _Ty & max(const _Ty &a, const _Ty &b, _LessComp less_comp)
```

Returns the greater of the given values. 



## Parameters
* *in* **a**

    The first value to compare. 

* *in* **b**

    The second value to compare. 

* *in* **less_comp**

    The user-defined less (<) comparison function used for comparing. 

## Return value
Returns the greater of the given values. Returns `a` if values are equivalent. 

