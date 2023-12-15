# Luna::strhash32

```c++
constexpr u32 strhash32(const c8 *s, u32 h=0)
```

## Overview
A specialization of strhash that computes 32-bit hash code. 

## Parameters
### s
A pointer to one null-terminated string to compute. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the string. 

