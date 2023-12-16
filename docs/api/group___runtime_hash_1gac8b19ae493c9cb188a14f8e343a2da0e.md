# Luna::memhash64

```c++
u64 memhash64(const void *data, usize size, u64 h=0)
```

A specialization of [memhash](group___runtime_hash_1gae0c40164557e718d6ee7b7c613210075.md) that computes 64-bit hash code. 

## Parameters
* *in* **data**

    A pointer to the data to be hashed. 

* *in* **size**

    The length of the data in bytes. 

* *in* **h**

    A initial hash value. See [memhash](group___runtime_hash_1gae0c40164557e718d6ee7b7c613210075.md) for details. 

## Return value
Returns the hash code of the data. 

