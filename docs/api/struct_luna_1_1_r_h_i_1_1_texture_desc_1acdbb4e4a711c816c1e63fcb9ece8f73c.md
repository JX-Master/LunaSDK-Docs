# Luna::RHI::TextureDesc::array_size

```c++
u32 array_size
```

The texture array size, specify 1 if this is not a texture array. This should always be 1 for 3D textures. This should be times of 6 of `usages` contains `TextureUsageFlag::cube`. 

