# Luna::Ref::operator<

```c++
bool operator<(const Ref &rhs) const
```

Compares two references. 

The referneces are compared by comparing their underlying pointers after comverted to unsigned integers. If the reference is not valid, the converted integer will be `0`. 

## Parameters
* *in* **rhs**

    The reference to compare with. 

## Return value
Returns `true` if this reference is less than the incoming reference. Returns `false` otherwise. 

