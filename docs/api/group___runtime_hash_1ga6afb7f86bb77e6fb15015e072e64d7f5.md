# Luna::strhash

```c++
template <typename _HashTy>
constexpr _HashTy strhash(const c8 *s, _HashTy h=0)
```

Computes a hash code for the specified string. 

## Overview


## Parameters
### s
A pointer to one null-terminated string to compute. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the string. 

