# Luna::memhash8

```c++
u8 memhash8(const void *data, usize size, u8 h=0)
```

A specialization of memhash that computes 8-bit hash code. 

## Parameters
### data
A pointer to the data to be hashed. 

### size
The length of the data in bytes. 

### h
A initial hash value. See memhash for details. 

## Return value
Returns the hash code of the data. 

