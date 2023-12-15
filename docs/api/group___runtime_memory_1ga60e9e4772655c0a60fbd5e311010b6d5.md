# Luna::memrealloc

```c++
LUNA_RUNTIME_API void * memrealloc(void *ptr, usize size, usize alignment=0)
```

Reallocates heap memory. 

## Overview


## Parameters
### ptr
The pointer to the former allocated memory block. If this is `nullptr`, this method behaves the same as memalloc. 

### size
The size, in bytes, of the new memory to allocate. If this is `0` and `ptr` is not `nullptr`, this function behaves the same as memfree. 

### alignment
Optional. The alignment requirement of the allocated memory block. Default is 0. memrealloc cannot change the alignment requirement of the memory block. In other words, if `ptr` is not `nullptr`, the alignment requirements of the old and new memory block must be the same. 

## Return value
Returns one pointer to the reallocated memory block. Returns `nullptr` if the allocation is failed. In such case, the old memory block (if have) is not changed.


This function allocates a new memory block with the specified size and alignment requirement, copies the data from the old memory block to the new one, and frees the old memory block. 

#### Valid Usage
* If `ptr` is not `nullptr`, `ptr` be allocated by a prior call to memalloc or memrealloc.

* If `ptr` is not `nullptr`, `alignment` be equal to `alignment` passed to memalloc or memrealloc which allocates `ptr`. 

