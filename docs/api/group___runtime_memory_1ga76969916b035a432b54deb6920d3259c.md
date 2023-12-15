# Luna::memalloc

```c++
LUNA_RUNTIME_API void * memalloc(usize size, usize alignment=0)
```

Allocates heap memory. 



## Parameters
### size
The size, in bytes, of the memory block to allocate. If this is `0`, no memory will be allocated. 

### alignment
Optional. The alignment requirement, in bytes, of the memory block to allocate. Default is `0`.


If this is 0 (default), then the memory is allocated with no additional alignment requirement. In such case, the memory address is aligned to 8 bytes in 32-bit platform, and 16 bytes in 64-bit platform.

## Return value
Returns one pointer to the allocated memory block. Returns `nullptr` if memory allocation failed or if `size` is `0`. 

#### Valid Usage
* If `alignment` is not `0`, `alignment` be powers of 2 (like 32, 64, 128, 256, etc). 

