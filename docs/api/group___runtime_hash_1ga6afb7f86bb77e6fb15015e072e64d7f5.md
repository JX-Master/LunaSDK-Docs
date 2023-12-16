# Luna::strhash

```c++
template <typename _HashTy>
constexpr _HashTy strhash(const c8 *s, _HashTy h=0)
```

Computes a hash code for the specified string. 



## Parameters
* *in* **s**

    A pointer to one null-terminated string to compute. 

* *in* **h**

    A initial hash value. See [memhash](group___runtime_hash_1gae0c40164557e718d6ee7b7c613210075.md) for details. 

## Return value
Returns the hash code of the string. 

