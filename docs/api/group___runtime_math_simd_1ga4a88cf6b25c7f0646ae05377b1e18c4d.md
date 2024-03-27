# Luna::Simd::load_f3x4

```c++
float3x4 load_f3x4(f32 const *mem_addr)
```

Loads 12 packed single-precision (32-bit) floating-point elements from `mem_addr` to `dst`. The highest 4 packed single-precision (32-bit) floating-point elements are uninitialized. 


```
FOR r := 0 to 2
       i := 128 * r
       dst[r].x := MEM[mem_addr + i : mem_addr + i + 31]
       dst[r].y := MEM[mem_addr + i + 32 : mem_addr + i + 63]
       dst[r].z := MEM[mem_addr + i + 64 : mem_addr + i + 95]
       dst[r].w := MEM[mem_addr + i + 96 : mem_addr + i + 127]
ENDFOR
```


