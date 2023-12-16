# Luna::memrealloc

```c++
void * memrealloc(void *ptr, usize size, usize alignment=0)
```

Reallocates heap memory. 



## Parameters
* *in* **ptr**

    The pointer to the former allocated memory block. If this is `nullptr`, this method behaves the same as [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md). 

* *in* **size**

    The size, in bytes, of the new memory to allocate. If this is `0` and `ptr` is not `nullptr`, this function behaves the same as [memfree](group___runtime_memory_1ga102bf0df13784b9f636c555461862a14.md). 

* *in* **alignment**

    Optional. The alignment requirement of the allocated memory block. Default is 0. [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md) cannot change the alignment requirement of the memory block. In other words, if `ptr` is not `nullptr`, the alignment requirements of the old and new memory block must be the same. 

## Return value
Returns one pointer to the reallocated memory block. Returns `nullptr` if the allocation is failed. In such case, the old memory block (if have) is not changed.


This function allocates a new memory block with the specified size and alignment requirement, copies the data from the old memory block to the new one, and frees the old memory block. 

## Valid Usage
* If `ptr` is not `nullptr`, `ptr`**must** be allocated by a prior call to [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md).

* If `ptr` is not `nullptr`, `alignment`**must** be equal to `alignment` passed to [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md) which allocates `ptr`. 

