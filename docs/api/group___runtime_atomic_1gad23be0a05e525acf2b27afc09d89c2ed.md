# Luna::atom_compare_exchange_usize

```c++
usize atom_compare_exchange_usize(usize volatile *dst, usize exchange, usize comperand)
```

Atomically compares the value of the variable with the specified comperand, and sets the variable to the specified value if equal. 



## Parameters
* *in* **dst**

    The pointer to the variable that needs to be compared. 

* *in* **exchange**

    The value to set to the variable if `*dst == comperand`. 

* *in* **comperand**

    The value to compare with. 

## Return value
Returns the value of the variable before this operation took place. 

## Remark
See remarks of [atom_compare_exchange_i32](group___runtime_atomic_1gaf678d9768b4d454a41fccf2b33eb1f2a.md) for details. 

