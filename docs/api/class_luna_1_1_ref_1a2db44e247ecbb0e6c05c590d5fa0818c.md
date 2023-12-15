# Luna::Ref::operator=

```c++
template <typename _Rty>
Ref & operator=(Ref< _Rty > &&rhs)
```

Assigns this reference by moving the pointer from another reference of one different type. 

The assignment will fail if the new reference is null or cannot be casted to `_Ty`. If the assignment fails, this reference will be null after this operation, and the strong reference counter of the new boxed object, if not null, will be decreased. If the assignment succeeds, the reference counter of the new boxed object will not be modified. The strong reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### rhs
The reference to move from. This reference will be null after this operation. 

## Return value
Returns `*this`. 

