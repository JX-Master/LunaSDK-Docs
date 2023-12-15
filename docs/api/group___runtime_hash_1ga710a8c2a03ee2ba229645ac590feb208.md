# Luna::memhash32

```c++
u32 memhash32(const void *data, usize size, u32 h=0)
```

## Overview
A specialization of memhash that computes 32-bit hash code. 

## Parameters
### data
A pointer to the data to be hashed. 

### size
The length of the data in bytes. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the data. 

