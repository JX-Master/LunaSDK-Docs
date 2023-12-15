# Luna::utf16_decode_char

```c++
LUNA_RUNTIME_API c32 utf16_decode_char(const c16 *str)
```

Decodes one Unicode character from 1~2 UTF-16 characters. 



## Parameters
### str
The pointer that points to UTF-16 characters to decode. 

## Return value
Returns the decoded Unicode character. 

#### Valid Usage
* `str` must points to a valid UTF-16 character string in platform-native endian. 

