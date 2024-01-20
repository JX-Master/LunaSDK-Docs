# Luna::Simd::load_f2

```c++
float4 load_f2(f32 const *mem_addr)
```

Loads 64-bits (composed of 2 packed single-precision (32-bit) floating-point elements) from memory into the first two elements of `dst`. The rest 2 elements are filled with 0. 


```
dst.x := MEM[mem_addr:mem_addr+31]
dst.y := MEM[mem_addr+32:mem_addr+63]
dst.z := 0
dst.w := 0
```


## Parameters
* *in* **mem_addr**

    The memory to load values. 

## Valid Usage
* `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

