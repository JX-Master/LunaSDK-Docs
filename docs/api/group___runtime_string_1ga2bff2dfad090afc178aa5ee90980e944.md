# Luna::strtou64

```c++
u64 strtou64(const c8 *str, c8 **str_end, i32 base)
```

Interprets an unsigned integer value in a string pointed to by `str`. 



## Parameters
* *in* **str**

    The pointer to the null-terminated byte string to be interpreted. 

* *out* **str_end**

    If not `nullptr`, returns the pointer to the end of the unsigned integer value string being interpreted. 

* *in* **base**

    The encoding base for the interpreted unsiged integer value. 

## Return value
Returns the converted value. If the converted value falls out of range of corresponding return type, `0` or [U64_MAX](group___runtime_base_type_1gac5d257d9894ee47f4445391853a0be72.md) is returned. If no conversion can be performed, `0`​ is returned. 

