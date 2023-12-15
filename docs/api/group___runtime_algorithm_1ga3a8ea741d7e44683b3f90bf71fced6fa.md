# Luna::min

```c++
template <typename _Ty, typename _LessComp>
constexpr const _Ty & min(const _Ty &a, const _Ty &b, _LessComp less_comp)
```

Returns the smaller of the given values. 

## Overview


## Parameters
### a
The first value to compare. 

### b
The second value to compare. 

### less_comp
The user-defined less (<) comparison function used for comparing. 

## Return value
Returns the smaller of the given values. Returns `a` if values are equivalent. 

