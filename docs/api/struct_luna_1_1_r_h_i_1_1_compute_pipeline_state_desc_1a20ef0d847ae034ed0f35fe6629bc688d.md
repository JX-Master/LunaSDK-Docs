# Luna::RHI::ComputePipelineStateDesc::metal_numthreads_x

```c++
u32 metal_numthreads_x
```

The number of threads in one thread group in X dimension for Metal backend. 

This is used only if the RHI backend is [BackendType::metal](group___r_h_i_1gga4da0d14d49c5f620d126d5cc3fdc2a33a86094b61cb9f63b77f982ceae03e95f0.md), since metal shader files does not include thread group size. 

