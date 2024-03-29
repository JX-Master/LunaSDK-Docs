# Luna::strtof64

```c++
f64 strtof64(const c8 *str, c8 **str_end)
```

Interprets a floating-point value in a string pointed to by `str`. 



## Parameters
* *in* **str**

    The pointer to the null-terminated byte string to be interpreted. 

* *out* **str_end**

    If not `nullptr`, returns the pointer to the end of the floating-point value string being interpreted. 

## Return value
Returns the converted value. If the converted value falls out of range of corresponding return type, [F64_INFINITY](group___runtime_math_1gab4ac7a7a782d35df2f1f174899eb10b6.md) is returned. If no conversion can be performed, `0`​ is returned. 

