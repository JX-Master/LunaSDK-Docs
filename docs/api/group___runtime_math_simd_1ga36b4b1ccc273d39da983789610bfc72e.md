# Luna::Simd::load_f4x4

```c++
float4x4 load_f4x4(f32 const *mem_addr)
```

Loads 16 packed single-precision (32-bit) floating-point elements from `mem_addr` to `dst`. `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 


```
FOR r := 0 to 3
       i := 128 * r
       dst[r].x := MEM[mem_addr + i : mem_addr + i + 31]
       dst[r].y := MEM[mem_addr + i + 32 : mem_addr + i + 63]
       dst[r].z := MEM[mem_addr + i + 64 : mem_addr + i + 95]
       dst[r].w := MEM[mem_addr + i + 96 : mem_addr + i + 127]
ENDFOR
```


