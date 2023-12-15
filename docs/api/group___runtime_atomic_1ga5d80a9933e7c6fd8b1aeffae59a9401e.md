# Luna::atom_dec_u32

```c++
u32 atom_dec_u32(u32 volatile *v)
```

Atomically decrease the value of the variable by 1. 

## Overview
This operation cannot be interrupted by system thread switching. 

## Parameters
### v
The pointer to the variable that needs to be changed. 

## Return value
Returns the value of the variable after this operation. 

