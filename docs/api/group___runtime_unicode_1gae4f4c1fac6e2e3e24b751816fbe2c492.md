# Luna::utf16_strlen

```c++
constexpr usize utf16_strlen(const c16 *src)
```

Gets the number of Unicode characters in a null-terminated UTF-16 string, not including the null terminator. 



## Parameters
* *in* **src**

    The UTF-16 string to check. 

## Return value
Returns the number of Unicode characters in the UTF-16 string. 

## Valid Usage
* `src` must points to a valid, null-terminated UTF-16 string. 

