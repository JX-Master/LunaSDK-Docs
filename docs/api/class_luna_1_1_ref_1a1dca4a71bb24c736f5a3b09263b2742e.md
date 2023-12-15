# Luna::Ref::operator=

```c++
template <typename _Rty>
Ref & operator=(const Ref< _Rty > &rhs)
```

Assigns this reference by coping the pointer from another reference of one different type. 

## Overview
The assignment will fail if the new reference is null or cannot be casted to `_Ty`. If the assignment fails, this reference will be null after this operation. If the assignment succeeds, The strong reference counter of the new boxed object will be increased. The strong reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### rhs
The reference to copy from. 

## Return value
Returns `*this`. 

