# Luna::UniquePtr::operator==

```c++
bool operator==(const UniquePtr &rhs) const
```

Compares two smart pointers for equality. Two smart pointers are equal if their native pointers are equal or both null. 



## Parameters
* *in* **rhs**

    The smart pointer to compare with. 

## Return value
Returns `true` if two smart pointers are equal. Returns `false` otherwise. 

## Remark
Since one native pointer can never be hold by two unique smart pointers at the same time (which causes double deletion), this is mainly used for comparing one smart pointer with `nullptr`. 

