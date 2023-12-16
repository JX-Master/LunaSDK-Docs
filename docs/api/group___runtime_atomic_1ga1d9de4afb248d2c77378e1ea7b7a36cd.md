# Luna::atom_exchange_i64

```c++
i64 atom_exchange_i64(i64 volatile *dst, i64 v)
```

Atomically replace the value of the variable with the value provided. 

This operation cannot be interrupted by system thread switching. 

## Parameters
* *in* **dst**

    The pointer to the variable that needs to be changed. 

* *in* **v**

    The value that needs to be set to the variable. 

## Return value
Returns the value of the variable before this operation took place. 

