# Luna::intern_name

```c++
const c8 * intern_name(const c8 *name, usize count)
```

Interns one name string to the runtime and fetches the interned address for it. 



## Parameters
### name
The name string to intern. 

### count
The number of characters that should be copied in `name`, excluding the null terminator if any. 

## Return value
Returns the interned address for the name string. If `name` is `nullptr` or `size` is `0`, the returned address is `nullptr` and the memory block is not interned. 

## Remark
The name string is saved in the runtime and is reference counted. The first call to intern_namewith a new string allocates the memory block to store the string and returns the block address. Additional calls to [intern_name](group___runtime_name_1gaa261ca6305ee4dee587492a004d6f9ee.md) with the same string will only increase the reference count of the memory block and returns the same address, so the user can simply compares two address (pointer) to check if they refer to the same string.


For each call to [intern_name](group___runtime_name_1gaa261ca6305ee4dee587492a004d6f9ee.md), one call to [release_name](group___runtime_name_1ga5556ed51beb79868d1c0f036ea3aa04d.md) is needed to finally release the internal name string block.

For end user, prefer using [Name](class_luna_1_1_name.md) objects instead of calling these APIs directly. 

