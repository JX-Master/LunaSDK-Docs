# Luna::intern_name

```c++
LUNA_RUNTIME_API const c8 * intern_name(const c8 *name, usize count)
```

Interns one name string to the runtime and fetches the interned address for it. 



## Parameters
### name
The name string to intern. 

### count
The number of characters that should be copied in `name`, excluding the null terminator if any. 

## Return value
Returns the interned address for the name string. If `name` is `nullptr` or `size` is `0`, the returned address is `nullptr` and the memory block is not interned. 


For each call to intern_name, one call to release_name is needed to finally release the internal name string block.

For end user, prefer using [Name](class_luna_1_1_name.md) objects instead of calling these APIs directly. 

