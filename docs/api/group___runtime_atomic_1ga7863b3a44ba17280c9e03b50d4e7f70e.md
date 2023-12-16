# Luna::atom_exchange_usize

```c++
usize atom_exchange_usize(usize volatile *dst, usize v)
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

