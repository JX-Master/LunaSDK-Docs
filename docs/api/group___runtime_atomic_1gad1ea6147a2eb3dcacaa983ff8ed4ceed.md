# Luna::atom_dec_usize

```c++
usize atom_dec_usize(usize volatile *v)
```

Atomically decrease the value of the variable by 1. 

This operation cannot be interrupted by system thread switching. 

## Parameters
* *in* **v**

    The pointer to the variable that needs to be changed. 

## Return value
Returns the value of the variable after this operation. 

