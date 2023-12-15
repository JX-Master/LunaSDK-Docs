# Luna::memnew

```c++
template <typename _Ty, typename...>
_Ty * memnew(_Args &&... args)
```

Allocates heap memory for one object and constructs the object. 

## Overview


## Return value
Returns one pointer to the allocated object. Returns `nullptr` if memory allocation failed. 

