# Luna::utf8_decode_char

```c++
c32 utf8_decode_char(const c8 *str)
```

Decodes one Unicode character from 1~6 UTF-8 characters. 



## Parameters
* *in* **str**

    The pointer that points to UTF-8 characters to decode. 

## Return value
Returns the decoded Unicode character. 

## Valid Usage
* `str` must points to a valid UTF-8 character string. 

