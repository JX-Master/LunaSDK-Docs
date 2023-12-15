# Luna::memhash64

```c++
u64 memhash64(const void *data, usize size, u64 h=0)
```

A specialization of memhash that computes 64-bit hash code. 

## Parameters
### data
A pointer to the data to be hashed. 

### size
The length of the data in bytes. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the data. 

