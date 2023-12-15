# Luna::strhash16

```c++
constexpr u16 strhash16(const c8 *s, u16 h=0)
```

A specialization of strhash that computes 16-bit hash code. 

## Parameters
### s
A pointer to one null-terminated string to compute. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the string. 

