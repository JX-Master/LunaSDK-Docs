# Luna::WeakObjRef::WeakObjRef

```c++
WeakObjRef(WeakObjRef &&rhs)
```

Constructs one reference by moving the pointer from another reference. 

## Overview
The weak reference counter of the new boxed object is not modified. 

## Parameters
### rhs
The reference to move from. This reference will be null after this operation. 

