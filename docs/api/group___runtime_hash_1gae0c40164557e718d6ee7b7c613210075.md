# Luna::memhash

```c++
template <typename _HashTy>
_HashTy memhash(const void *data, usize size, _HashTy h=0)
```

Computes a hash code for the specified binary data. 

This is the basic hash function that uses crc32 hash algorithm to hash any kind of binary data stream to a single hash value. 

## Parameters
* *in* **data**

    A pointer to the data to be hashed. 

* *in* **size**

    The length of the data in bytes. 

* *in* **h**

    A initial hash value. If this is a new hash, set to 0 (which is the default value if not specified). If this is a rehash operation or a second have before another one, you can specify the last hash value to get a different hash value from the same data. 

## Return value
Returns the hash code of the data. 

