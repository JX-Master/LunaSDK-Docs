# Luna::strhash8

```c++
constexpr u8 strhash8(const c8 *s, u8 h=0)
```

A specialization of [strhash](group___runtime_hash_1ga6afb7f86bb77e6fb15015e072e64d7f5.md) that computes 8-bit hash code. 



## Parameters
* *in* **s**

    A pointer to one null-terminated string to compute. 

* *in* **h**

    A initial hash value. See [memhash](group___runtime_hash_1gae0c40164557e718d6ee7b7c613210075.md) for details. 

## Return value
Returns the hash code of the string. 

