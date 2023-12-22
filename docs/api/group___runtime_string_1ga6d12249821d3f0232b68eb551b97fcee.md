# Luna::strtof32

```c++
f32 strtof32(const c8 *str, c8 **str_end)
```

Interprets a floating-point value in a string pointed to by `str`. 



## Parameters
* *in* **str**

    The pointer to the null-terminated byte string to be interpreted. 

* *out* **str_end**

    If not `nullptr`, returns the pointer to the end of the floating-point value string being interpreted. 

## Return value
Returns the converted value. If the converted value falls out of range of corresponding return type, F32_INFINITY is returned. If no conversion can be performed, `0`​ is returned. 

