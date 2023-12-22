# Luna::strtoi64

```c++
i64 strtoi64(const c8 *str, c8 **str_end, i32 base)
```

Interprets an integer value in a string pointed to by `str`. 



## Parameters
* *in* **str**

    The pointer to the null-terminated byte string to be interpreted. 

* *out* **str_end**

    If not `nullptr`, returns the pointer to the end of the integer value string being interpreted. 

* *in* **base**

    The encoding base for the interpreted integer value. 

## Return value
Returns the converted value. If the converted value falls out of range of corresponding return type, [I64_MIN](group___runtime_base_type_1gabd21eb34dd9332cb66e64ca7b1aebd47.md) or [I64_MAX](group___runtime_base_type_1gab02a9a57710d480fd593c00b8d7c71d9.md) is returned. If no conversion can be performed, `0`​ is returned. 

