# Luna::utf16_encode_char

```c++
usize utf16_encode_char(c16 *dst, c32 ch)
```

Encodes the Unicode character into 1~2 UTF-16 characters using platform-native endian. 



## Parameters
### dst
The buffer for writing encoded UTF-16 characters. 

### ch
The Unicode character to encode. 

## Return value
Returns the number of UTF-16 characters written to `dst`. 

## Valid Usage
* `dst` must be large enough to hold all UTF-16 characters written. The user can use [utf16_charspan](group___runtime_unicode_1gaee1dfeafcf1e5b2e0abfded74899f3c6.md) to check the required space in advance. 

