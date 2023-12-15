# Luna::utf8_to_utf16_len

```c++
LUNA_RUNTIME_API usize utf8_to_utf16_len(const c8 *src, usize src_chars=USIZE_MAX)
```

Determines the length of the corresponding UTF-16 string for a UTF-8 string, not include the null-terminator. 

## Overview


## Parameters
### src
The UTF-8 string to check. 

### src_chars
The maximum characters to read. Specify `USIZE_MAX` to read till the end of the string. The checking process will stop on first null terminator, or when `src_chars` is reached. 

## Return value
Returns the length of the corresponding UTF-16 string for a UTF-8 string, not include the null-terminator. 
