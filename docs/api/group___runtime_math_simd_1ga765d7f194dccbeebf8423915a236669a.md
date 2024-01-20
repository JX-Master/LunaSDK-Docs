# Luna::Simd::store_f2

```c++
void store_f2(f32 *mem_addr, float4 a)
```

Stores the lower 2 single-precision (32-bit) floating-point elements from `a` into memory. 


```
MEM[mem_addr:mem_addr+31] := a.x
MEM[mem_addr+32:mem_addr+63] := a.y
```


## Parameters
* *in* **mem_addr**

    The memory to store values. 

* *in* **a**

    The value to store. 

## Valid Usage
* `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

