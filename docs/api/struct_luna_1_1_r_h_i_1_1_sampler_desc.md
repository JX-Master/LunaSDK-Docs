# Luna::RHI::SamplerDesc
Describes one sampler in descriptor set. 

```c++
struct Luna::RHI::SamplerDesc
```

## Member objects
* [Filter min_filter](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a201fe5a47857ba61ef4fb670152527e4.md)

    The filter applied when the sample pixel size is greater than texel. 

* [Filter mag_filter](struct_luna_1_1_r_h_i_1_1_sampler_desc_1ad88bf364d5119c107d67d229426b0896.md)

    The filter applied when the sample pixel size is smaller than texel. 

* [Filter mip_filter](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a44b3ca87bde5aab6615ff1ba6139757e.md)

    The filter applied when sampling between different mipmaps. 

* [TextureAddressMode address_u](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a9cbd91eb0ca9367e021b02d7f42da094.md)

    The address mode used in the first direction (from left to right). 

* [TextureAddressMode address_v](struct_luna_1_1_r_h_i_1_1_sampler_desc_1afb055bde450ce94db875aca0e5eea6ed.md)

    The address mode used in the second direction (from top to down in D3D/Vulkan, from down to top in Metal). 

* [TextureAddressMode address_w](struct_luna_1_1_r_h_i_1_1_sampler_desc_1af472e53a9a1ba835541d31727d9a4cad.md)

    The address mode used in the third direction (from front to back in 3D textures). 

* [bool anisotropy_enable](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a1e8c7c3ebf6eabf931a232e5842f8c05.md)

    Whether to enable anisotropy sampling. 

* [bool compare_enable](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a66243f5825dbba80905b50799c349f19.md)

    Whether to enable pixel comparing. 

* [CompareFunction compare_function](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a0e1051c7f0e24a68342e5749d136efd0.md)

    The compare function used when `compare_enable` is `true`. 

* [BorderColor border_color](struct_luna_1_1_r_h_i_1_1_sampler_desc_1ae0c693c9793a6341f2df24b472def168.md)

    The border color used when `TextureAddressMode::border` is set. 

* [u32 max_anisotropy](struct_luna_1_1_r_h_i_1_1_sampler_desc_1afa01ec18ff46dda2d17f8a742f8bcb42.md)

    The maximum anisotropy ratio. 

* [f32 min_lod](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a0efbf62641b790b6ddb2d87de8798119.md)

    The minimum LOD level that will be sampled. 

* [f32 max_lod](struct_luna_1_1_r_h_i_1_1_sampler_desc_1a9dd5087efe1b6cd9bb7b8db3a0cdc3c5.md)

    The maximum LOD level that will be sampled. Specify one large enough value (like F32_MAX) to disable this limit. 

