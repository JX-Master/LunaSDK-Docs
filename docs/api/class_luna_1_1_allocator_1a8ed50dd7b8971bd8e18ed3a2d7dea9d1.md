# Luna::Allocator::allocate

```c++
template <typename _Ty>
_Ty * allocate(usize n=1)
```

Allocates memory for the specified number of elements. 



## Parameters
### n
The number of elements to allocate memory for. 

## Return value
Returns the allocated memory. The size of the allocated memory is at least `sizeof(_Ty) * n` bytes, and the alignment of the allocated memory is at least `alignof(_Ty)` bytes. The returned memory is uninitialized. If the allocation fails, returns `nullptr`. 

