# Luna::strhash64

```c++
constexpr u64 strhash64(const c8 *s, u64 h=0)
```

A specialization of strhash that computes 64-bit hash code. 

## Parameters
### s
A pointer to one null-terminated string to compute. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the string. 

