# Luna::utf8_encode_char

```c++
LUNA_RUNTIME_API usize utf8_encode_char(c8 *dst, c32 ch)
```

Encodes the Unicode character into 1~6 UTF-8 characters. 

## Overview


## Parameters
### dst
The buffer for writing encoded UTF-8 characters. 

### ch
The Unicode character to encode. 

## Return value
Returns the number of UTF-8 characters written to `dst`. 

#### Valid Usage
* `dst` must be large enough to hold all UTF-8 characters written. The user can use utf8_charspan to check the required space in advance. 
