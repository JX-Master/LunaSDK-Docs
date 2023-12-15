# Luna::atom_add_u32

```c++
u32 atom_add_u32(u32 volatile *base, i32 v)
```

Atomically increase the value of the variable by the the value provided. 

This operation cannot be interrupted by system thread switching. 

## Parameters
### base
The pointer to the variable that needs to be changed. 

### v
The value that needs to be added to the variable. 

## Return value
Returns the value of the variable before this operation. 

