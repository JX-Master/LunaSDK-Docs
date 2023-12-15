# Luna::memsize

```c++
LUNA_RUNTIME_API usize memsize(void *ptr, usize alignment=0)
```

Gets the allocated size of one memory block. 

## Overview


## Parameters
### ptr
The pointer to the memory block. 

### alignment
Optional. The alignment requirement of the allocated memory block. Default is 0. 

## Return value
Returns the size of bytes of the memory block. Returns `0` if `ptr` is `nullptr`.


The returned size is the size allocated for the memory block and is available for the user to use. The allocated size may be larger than the required size passed to memalloc or memrealloc to satisfy alignment and padding requirements. 

#### Valid Usage
* If `ptr` is not `nullptr`, `ptr` be allocated by a prior call to memalloc or memrealloc.

* If `ptr` is not `nullptr`, `alignment` be equal to `alignment` passed to memalloc or memrealloc which allocates `ptr`. 

