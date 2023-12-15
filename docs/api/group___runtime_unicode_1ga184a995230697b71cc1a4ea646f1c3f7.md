# Luna::utf8_index

```c++
constexpr usize utf8_index(const c8 *str, usize n)
```

Gets the index of the first UTF-8 character for the specified Unicode character. 

## Overview


## Parameters
### str
The UTF-8 string to check. 

### n
The index of the Unicode character to check. 

## Return value
Returns the index of the first UTF-8 character for the specified Unicode character. 

#### Valid Usage
* `src` must points to a valid UTF-8 string.

* `n` must be smaller than the number of Unicode characters in the string. 

