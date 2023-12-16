# Luna::memrealloc

```c++
void * memrealloc(void *ptr, usize size, usize alignment=0)
```

Reallocates heap memory. 



## Parameters
### ptr
The pointer to the former allocated memory block. If this is `nullptr`, this method behaves the same as [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md). 

### size
The size, in bytes, of the new memory to allocate. If this is `0` and `ptr` is not `nullptr`, this function behaves the same as [memfree](group___runtime_memory_1ga4bc8f37f2fe8c9100a8af16de794e3de.md). 

### alignment
Optional. The alignment requirement of the allocated memory block. Default is 0. [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md) cannot change the alignment requirement of the memory block. In other words, if `ptr` is not `nullptr`, the alignment requirements of the old and new memory block must be the same. 

## Return value
Returns one pointer to the reallocated memory block. Returns `nullptr` if the allocation is failed. In such case, the old memory block (if have) is not changed.


This function allocates a new memory block with the specified size and alignment requirement, copies the data from the old memory block to the new one, and frees the old memory block. 

## Valid Usage
* If `ptr` is not `nullptr`, `ptr` be allocated by a prior call to [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md).

* If `ptr` is not `nullptr`, `alignment` be equal to `alignment` passed to [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md) which allocates `ptr`. 

