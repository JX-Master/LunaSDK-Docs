# Luna::utf16_encode_char

```c++
LUNA_RUNTIME_API usize utf16_encode_char(c16 *dst, c32 ch)
```

Encodes the Unicode character into 1~2 UTF-16 characters using platform-native endian. 

## Overview


## Parameters
### dst
The buffer for writing encoded UTF-16 characters. 

### ch
The Unicode character to encode. 

## Return value
Returns the number of UTF-16 characters written to `dst`. 

#### Valid Usage
* `dst` must be large enough to hold all UTF-16 characters written. The user can use utf16_charspan to check the required space in advance. 

