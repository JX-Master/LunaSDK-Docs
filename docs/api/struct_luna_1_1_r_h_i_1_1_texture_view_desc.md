# Luna::RHI::TextureViewDesc
Describes one texture view in descriptor set. 

```c++
struct Luna::RHI::TextureViewDesc
```

## Member objects
* [ITexture* texture](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1ab02abc67d0395436de0c53aca08fd08f.md)

    The texture to set. 

* [TextureViewType type](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1a4550d2ae4c182b2cf10aebc3ef743a68.md)

    The texture view type. If this is [TextureViewType::unspecified](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9ad415f0e30c471dfdd9bc4f827329ef48.md), the system uses the texture's native type as texture view type. 

* [Format format](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1a751c4987b2c6908c70a915ab18d36653.md)

    The texture view format. If this is Format::unknown, the system uses the texture's native format as texture view format. 

* [u32 mip_slice](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1a6d27e4a4383c82f0fd25d296517f3b8b.md)

    The index of the first mip included in this view. 

* [u32 mip_size](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1a6a986116c17f1cd09629b757dd3771c7.md)

    The number of mips included in this view. Mips in range [`mip_slice`, `mip_slice + mip_size`) will be included in this view. 

* [u32 array_slice](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1af0b0cad0aa42b5145951ecd38a2d88ee.md)

    The index of the first texture array element included in this view. 

* [u32 array_size](struct_luna_1_1_r_h_i_1_1_texture_view_desc_1acdbb4e4a711c816c1e63fcb9ece8f73c.md)

    The number of array elements included in this view. [Array](class_luna_1_1_array.md) elements in range [`array_slice`, `array_slice + array_size`) will be included in this view. 

