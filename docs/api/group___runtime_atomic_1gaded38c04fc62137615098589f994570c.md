# Luna::atom_add_usize

```c++
usize atom_add_usize(usize volatile *base, isize v)
```

Atomically increase the value of the variable by the the value provided. 

This operation cannot be interrupted by system thread switching. 

## Parameters
* *in* **base**

    The pointer to the variable that needs to be changed. 

* *in* **v**

    The value that needs to be added to the variable. 

## Return value
Returns the value of the variable before this operation. 

