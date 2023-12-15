# Luna::Simd::float4x4
```c++
struct Luna::Simd::float4x4
```

## Overview
Represents one SIMD matrix type with 16 (4x4) packed single-precision (32-bit) floating-point elements. Based on the implementation, the matrix may be stored using two 256-bits registers (AVX), or four 128-bits registers (SSEn / Neon). 

