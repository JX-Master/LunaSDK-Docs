# Luna::strhash8

```c++
constexpr u8 strhash8(const c8 *s, u8 h=0)
```

A specialization of strhash that computes 8-bit hash code. 

## Parameters
### s
A pointer to one null-terminated string to compute. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the string. 

