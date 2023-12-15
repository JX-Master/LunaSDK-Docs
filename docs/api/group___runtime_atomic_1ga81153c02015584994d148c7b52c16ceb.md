# Luna::atom_compare_exchange_pointer

```c++
template <typename _Ty>
_Ty * atom_compare_exchange_pointer(_Ty *volatile *dst, void *exchange, void *comperand)
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

