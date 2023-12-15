# Luna::atom_exchange_u64

```c++
u64 atom_exchange_u64(u64 volatile *dst, u64 v)
```

Atomically replace the value of the variable with the value provided. 

This operation cannot be interrupted by system thread switching. 

## Parameters
### dst
The pointer to the variable that needs to be changed. 

### v
The value that needs to be set to the variable. 

## Return value
Returns the value of the variable before this operation took place. 

