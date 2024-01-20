# Luna::Simd::store_f4

```c++
void store_f4(f32 *mem_addr, float4 a)
```

Stores 128-bits (composed of 4 packed single-precision (32-bit) floating-point elements) from `a` into memory. 


```
MEM[mem_addr:mem_addr+31] := a.x
MEM[mem_addr+32:mem_addr+63] := a.y
MEM[mem_addr+64:mem_addr+95] := a.z
MEM[mem_addr+96:mem_addr+127] := a.w
```


## Parameters
* *in* **mem_addr**

    The memory to store values. 

* *in* **a**

    The value to store. 

## Valid Usage
* `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

