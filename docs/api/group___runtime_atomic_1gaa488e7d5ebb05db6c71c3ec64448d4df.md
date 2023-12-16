# Luna::atom_inc_u64

```c++
u64 atom_inc_u64(u64 volatile *v)
```

Atomically increase the value of the variable by 1. 

This operation cannot be interrupted by system thread switching. 

## Parameters
* *in* **v**

    The pointer to the variable that needs to be changed. 

## Return value
Returns the value of the variable after this operation. 

