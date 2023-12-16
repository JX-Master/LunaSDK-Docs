# Luna::memsize

```c++
usize memsize(void *ptr, usize alignment=0)
```

Gets the allocated size of one memory block. 



## Parameters
### ptr
The pointer to the memory block. 

### alignment
Optional. The alignment requirement of the allocated memory block. Default is 0. 

## Return value
Returns the size of bytes of the memory block. Returns `0` if `ptr` is `nullptr`.


The returned size is the size allocated for the memory block and is available for the user to use. The allocated size may be larger than the required size passed to [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md) to satisfy alignment and padding requirements. 

## Valid Usage
* If `ptr` is not `nullptr`, `ptr` be allocated by a prior call to [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md).

* If `ptr` is not `nullptr`, `alignment` be equal to `alignment` passed to [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md) which allocates `ptr`. 

