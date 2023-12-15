# Luna::atom_add_i64

```c++
i64 atom_add_i64(i64 volatile *base, i64 v)
```

Atomically increase the value of the variable by the the value provided. 

## Overview
This operation cannot be interrupted by system thread switching. 

## Parameters
### base
The pointer to the variable that needs to be changed. 

### v
The value that needs to be added to the variable. 

## Return value
Returns the value of the variable before this operation. 

