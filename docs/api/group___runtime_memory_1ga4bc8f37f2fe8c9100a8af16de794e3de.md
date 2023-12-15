# Luna::memfree

```c++
LUNA_RUNTIME_API void memfree(void *ptr, usize alignment=0)
```

Frees heap memory. 

## Overview


## Parameters
### ptr
The pointer returned by memalloc or memrealloc. If this is `nullptr`, this function does nothing. 

### alignment
Optional. The alignment requirement specified when allocating the memory block. Default is 0. 

#### Valid Usage
* If `ptr` is not `nullptr`, `alignment` be equal to `alignment` passed to memalloc or memrealloc which allocates `ptr`. 

