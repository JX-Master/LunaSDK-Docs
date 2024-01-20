# Luna::Simd::load_f4

```c++
float4 load_f4(f32 const *mem_addr)
```

Loads 128-bits (composed of 4 packed single-precision (32-bit) floating-point elements) from memory into `dst`. 


```
dst.x := MEM[mem_addr:mem_addr+31]
dst.y := MEM[mem_addr+32:mem_addr+63]
dst.z := MEM[mem_addr+64:mem_addr+95]
dst.w := MEM[mem_addr+96:mem_addr+127]
```


## Valid Usage
* `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 

