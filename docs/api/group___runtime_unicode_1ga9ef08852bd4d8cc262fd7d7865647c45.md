# Luna::utf16_index

```c++
constexpr usize utf16_index(const c16 *str, usize n)
```

Gets the index of the first UTF-16 character for the specified Unicode character. 

## Overview


## Parameters
### str
The UTF-16 string to check. 

### n
The index of the Unicode character to check. 

## Return value
Returns the index of the first UTF-16 character for the specified Unicode character. 

#### Valid Usage
* `src` must points to a valid UTF-16 string.

* `n` must be smaller than the number of Unicode characters in the string. 

