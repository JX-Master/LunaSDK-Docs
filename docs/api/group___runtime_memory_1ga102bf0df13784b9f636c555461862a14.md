# Luna::memfree

```c++
void memfree(void *ptr, usize alignment=0)
```

Frees heap memory. 



## Parameters
* *in* **ptr**

    The pointer returned by [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md). If this is `nullptr`, this function does nothing. 

* *in* **alignment**

    Optional. The alignment requirement specified when allocating the memory block. Default is 0. 

## Valid Usage
* If `ptr` is not `nullptr`, `alignment`**must** be equal to `alignment` passed to [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md) which allocates `ptr`. 

