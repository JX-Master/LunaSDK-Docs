# Luna::Ref::operator=

```c++
Ref & operator=(Ref &&rhs)
```

Assigns this reference by moving the pointer from another reference of the same type. 

The reference counter of the new boxed object is not modified. The strong reference counter of the original boxed object, if not null, will be decreased before assignment. 

## Parameters
### rhs
The reference to move from. This reference will be null after this operation. 

## Return value
Returns `*this`. 

