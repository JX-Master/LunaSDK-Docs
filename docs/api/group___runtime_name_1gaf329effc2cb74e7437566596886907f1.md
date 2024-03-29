# Luna::intern_name

```c++
const c8 * intern_name(const c8 *name)
```

Interns one name string to the runtime and fetches the interned address for it. 



## Parameters
* *in* **name**

    The name string to intern. 

## Return value
Returns the interned address for the name string. If `name` is `nullptr` or points to an empty string (`""`), the returned address is `nullptr` and the memory block is not interned. 

## Remark
The name string is saved in the runtime and is reference counted. The first call to [intern_name](group___runtime_name_1gaf329effc2cb74e7437566596886907f1.md) with a new string allocates the memory block to store the string and returns the block address. Additional calls to [intern_name](group___runtime_name_1gaf329effc2cb74e7437566596886907f1.md) with the same string will only increase the reference count of the memory block and returns the same address, so the user can simply compares two address (pointer) to check if they refer to the same string.


For each call to [intern_name](group___runtime_name_1gaf329effc2cb74e7437566596886907f1.md), one call to [release_name](group___runtime_name_1ga752306e6c9de3a73e7eac1d2945880a0.md) is needed to finally release the internal name string block.

For end user, prefer using [Name](class_luna_1_1_name.md) objects instead of calling these APIs directly. 

## Valid Usage
* If `name` is not `nullptr`, it must be ended with one null terminator. 

