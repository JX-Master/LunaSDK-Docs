# Luna::Simd::store_f3x4

```c++
void store_f3x4(f32 *mem_addr, float3x4 m)
```

Stores the first 12 packed single-precision (32-bit) floating-point elements from `m` to `dst`. `mem_addr` must be aligned on a 16-byte boundary or a general-protection exception may be generated. 


```
FOR r := 0 to 2
    i := 128 * r
    MEM[mem_addr + i : mem_addr + i + 31] := m[r].x
    MEM[mem_addr + i + 32 : mem_addr + i + 63] := m[r].y
    MEM[mem_addr + i + 64 : mem_addr + i + 95] := m[r].z
    MEM[mem_addr + i + 96 : mem_addr + i + 127] := m[r].w
ENDFOR
```


