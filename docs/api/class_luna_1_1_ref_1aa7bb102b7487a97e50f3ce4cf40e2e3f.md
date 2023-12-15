# Luna::Ref::Ref

```c++
Ref(ObjRef &&rhs)
```

Constructs one reference by moving the pointer from one typeless reference. 

## Overview
The assignment will fail if the new reference is null or cannot be casted to `_Ty`. If the assignment fails, this reference will be null after this operation, and the strong reference counter of the new boxed object, if not null, will be decreased. If the assignment succeeds, the reference counter of the new boxed object will not be modified. 

## Parameters
### rhs
The reference to move from. This reference will be null after this operation. 

