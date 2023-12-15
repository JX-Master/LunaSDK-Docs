# Luna::atom_dec_i64

```c++
i64 atom_dec_i64(i64 volatile *v)
```

Atomically decrease the value of the variable by 1. 

## Overview
This operation cannot be interrupted by system thread switching. 

## Parameters
### v
The pointer to the variable that needs to be changed. 

## Return value
Returns the value of the variable after this operation. 

