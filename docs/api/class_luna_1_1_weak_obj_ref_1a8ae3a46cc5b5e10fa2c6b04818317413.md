# Luna::WeakObjRef::operator==

```c++
bool operator==(const WeakObjRef &rhs) const
```

Compares two references for equality. 

Two references are equal if their underlying pointers are either equal or both invalid. 

## Parameters
* *in* **rhs**

    The reference to compare with. 

## Return value
Returns `true` if two references are equal. Returns `false` otherwise. 

