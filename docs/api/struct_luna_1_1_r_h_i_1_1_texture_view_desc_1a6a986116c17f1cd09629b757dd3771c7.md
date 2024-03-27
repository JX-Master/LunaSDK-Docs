# Luna::RHI::TextureViewDesc::mip_size

```c++
u32 mip_size
```

The number of mips included in this view. Mips in range [`mip_slice`, `mip_slice + mip_size`) will be included in this view. 

If this is [U32_MAX](group___runtime_base_type_1ga645ed2bd2baa2b4ed82d67bc5597ef47.md), all mips beginning from `mip_slice` will be included in this view. 

