# Luna::atom_inc_i32

```c++
i32 atom_inc_i32(i32 volatile *v)
```

Atomically increase the value of the variable by 1. 

## Overview
This operation cannot be interrupted by system thread switching. 

## Parameters
### v
The pointer to the variable that needs to be changed. 

## Return value
Returns the value of the variable after this operation. 

