# Luna::memsize

```c++
usize memsize(void *ptr, usize alignment=0)
```

Gets the allocated size of one memory block. 



## Parameters
* *in* **ptr**

    The pointer to the memory block. 

* *in* **alignment**

    Optional. The alignment requirement of the allocated memory block. Default is 0. 

## Return value
Returns the size of bytes of the memory block. Returns `0` if `ptr` is `nullptr`.


The returned size is the size allocated for the memory block and is available for the user to use. The allocated size may be larger than the required size passed to [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md) to satisfy alignment and padding requirements. 

## Valid Usage
* If `ptr` is not `nullptr`, `ptr`**must** be allocated by a prior call to [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md).

* If `ptr` is not `nullptr`, `alignment`**must** be equal to `alignment` passed to [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md) or [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md) which allocates `ptr`. 

