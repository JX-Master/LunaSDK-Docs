# Luna::WeakRef::operator!=

```c++
bool operator!=(const WeakRef &rhs) const
```

Compares two references for non-equality. 

Two references are equal if their underlying pointers are either equal or both invalid. 

## Parameters
* *in* **rhs**

    The reference to compare with. 

## Return value
Returns `true` if two references are not equal. Returns `false` otherwise. 

