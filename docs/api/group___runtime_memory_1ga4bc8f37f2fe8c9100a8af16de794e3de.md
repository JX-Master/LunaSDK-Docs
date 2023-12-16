# Luna::memfree

```c++
void memfree(void *ptr, usize alignment=0)
```

Frees heap memory. 



## Parameters
### ptr
The pointer returned by [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md). If this is `nullptr`, this function does nothing. 

### alignment
Optional. The alignment requirement specified when allocating the memory block. Default is 0. 

## Valid Usage
* If `ptr` is not `nullptr`, `alignment` be equal to `alignment` passed to [memalloc](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md) or [memrealloc](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md) which allocates `ptr`. 

