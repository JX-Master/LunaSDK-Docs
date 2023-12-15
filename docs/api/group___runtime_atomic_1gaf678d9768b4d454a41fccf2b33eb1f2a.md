# Luna::atom_compare_exchange_i32

```c++
i32 atom_compare_exchange_i32(i32 volatile *dst, i32 exchange, i32 comperand)
```

Atomically compares the value of the variable with the specified comperand, and sets the variable to the specified value if equal. 

## Overview


## Parameters
### dst
The pointer to the variable that needs to be compared. 

### exchange
The value to set to the variable if `*dst == comperand`. 

### comperand
The value to compare with. 

## Return value
Returns the value of the variable before this operation took place. 

