# Luna::Simd::float3x4
Represents one SIMD matrix type with 12 (3x4) packed single-precision (32-bit) floating-point elements. Based on the implementation, the matrix may be stored using two 256-bits registers (AVX), or four 128-bits registers (SSEn / Neon). 

```c++
struct Luna::Simd::float3x4
```

