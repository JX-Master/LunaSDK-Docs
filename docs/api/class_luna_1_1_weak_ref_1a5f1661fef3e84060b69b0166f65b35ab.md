# Luna::WeakRef::operator<

```c++
bool operator<(const WeakRef &rhs) const
```

Compares two references. 

## Overview
The referneces are compared by comparing their underlying pointers after converted to unsigned integers. If the reference is not valid, the converted integer will be `0`. 

## Parameters
### rhs
The reference to compare with. 

## Return value
Returns `true` if this reference is less than the incoming reference. Returns `false` otherwise. 

