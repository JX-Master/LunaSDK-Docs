# Luna::bit_set

```c++
void bit_set(void *addr, usize bit_offset, bool value)
```

Sets the specified bit to 1 if `value` is `true`, or to 0 if `value` is `false`. 



## Parameters
* *in* **base_addr**

    The address of the bit to offset from. 

* *in* **bit_offset**

    The number of bits shifted from the `base_addr`. 

* *in* **value**

    The value to set for the bit. 

## Remark
See remarks of [bit_test](group___runtime_memory_utils_1gaacaed16341185899ffe0d769237104f2.md) for details. 

