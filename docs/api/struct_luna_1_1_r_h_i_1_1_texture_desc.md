# Luna::RHI::TextureDesc
Describes one texture resource. 

```c++
struct Luna::RHI::TextureDesc
```

## Member objects
* [TextureType type](struct_luna_1_1_r_h_i_1_1_texture_desc_1a6d0659bb23ff72a9d7acd1ff2745b82b.md)

    The type of the texture. 

* [Format format](struct_luna_1_1_r_h_i_1_1_texture_desc_1a751c4987b2c6908c70a915ab18d36653.md)

    The pixel format of the texture. 

* [u32 width](struct_luna_1_1_r_h_i_1_1_texture_desc_1a85db88ffee2944ecd35c616393976289.md)

    The width of the texture. 

* [u32 height](struct_luna_1_1_r_h_i_1_1_texture_desc_1add40f8a56ae8cc650f92a3aa4d2bac99.md)

    The height of the texture. This should always be 1 for 1D textures. 

* [u32 depth](struct_luna_1_1_r_h_i_1_1_texture_desc_1aebf034dca5d4441f3b12bc2aaa9af93c.md)

    The depth of the texture. This should always be 1 for 1D and 2D textures. 

* [u32 array_size](struct_luna_1_1_r_h_i_1_1_texture_desc_1acdbb4e4a711c816c1e63fcb9ece8f73c.md)

    The texture array size, specify 1 if this is not a texture array. This should always be 1 for 3D textures. This should be times of 6 of `usages` contains `TextureUsageFlag::cube`. 

* [u32 mip_levels](struct_luna_1_1_r_h_i_1_1_texture_desc_1a22d014d788189a78f244c0755a1605b0.md)

    The number of mip-map slices. Specify 0 tells the system to create full mip-map chain for the resource. 

* [u32 sample_count](struct_luna_1_1_r_h_i_1_1_texture_desc_1a1c8270d54620086aa497d8d7ee065458.md)

    The sample count per pixel for multi-sample texture resource, specify 1 if the multi-sample is disabled for this texture. This should always be 1 for 1D and 3D textures. 

* [TextureUsageFlag usages](struct_luna_1_1_r_h_i_1_1_texture_desc_1afc94821d51b7c41bcb1fee1658b82285.md)

    A combination of `TextureUsageFlag` flags to indicate all possible usages of this texture. 

* [ResourceFlag flags](struct_luna_1_1_r_h_i_1_1_texture_desc_1a594bd04420fa22ac6308d9958fd3cb8b.md)

    The resource flags. 

