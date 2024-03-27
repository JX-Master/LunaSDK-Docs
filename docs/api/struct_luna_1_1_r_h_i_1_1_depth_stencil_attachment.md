# Luna::RHI::DepthStencilAttachment
Describes one depth stencil attachment when beginning a render pass. 

```c++
struct Luna::RHI::DepthStencilAttachment
```

## Member objects
* [ITexture* texture](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1ab02abc67d0395436de0c53aca08fd08f.md)

    The texture to bind for this attachment. The texture must have [TextureUsageFlag::depth_stencil_attachment](group___r_h_i_1gga158288d119b258c9a2dc7c2ca0cd2501a51ddd95056b201e7d04400cfcfeb4dfd.md) being set. 

* [LoadOp depth_load_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1a24930800f916fa1c5c947d034eda736b.md)

    The load operation to perform for depth component when reading data from attachment. 

* [StoreOp depth_store_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1abdf185983e540d1ee43bd077142162c2.md)

    The store operation to perform for depth component when writing data to attachment. 

* [LoadOp stencil_load_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1a410b830a5ad72ec10c22953a9fc3ea68.md)

    The load operation to perform for stencil component when reading data from attachment. 

* [StoreOp stencil_store_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1ac345b3cd44d063f61251536ded2c4c67.md)

    The store operation to perform for stencil component when writing data to attachment. 

* [f32 depth_clear_value](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1a94655a545d4c250baeab4db34825f2e9.md)

    The depth clear value to use if `depth_load_op` is [LoadOp::clear](group___r_h_i_1gga8d353cef0bd83ad8a6b73532498b26eea01bc6f8efa4202821e95f4fdf6298b30.md). Otherwise this value is ignored. 

* [u8 stencil_clear_value](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1ae58bd1a532a37a936291470f9e744930.md)

    The stencil clear value to use if `stencil_load_op` is [LoadOp::clear](group___r_h_i_1gga8d353cef0bd83ad8a6b73532498b26eea01bc6f8efa4202821e95f4fdf6298b30.md). Otherwise this value is ignored. 

* [bool read_only](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1ae851b490bae2ad91e401b972664fde81.md)

    Whether this is a read-only depth stencil attachment. 

* [TextureViewType view_type](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1acd11f9e113324f80f5cdfc92570490e9.md)

    The texture view type to view the texture as an attachment. If [TextureViewType::unspecified](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9ad415f0e30c471dfdd9bc4f827329ef48.md) is set, the system loads the texture's texture type as view type. 

* [Format format](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1a751c4987b2c6908c70a915ab18d36653.md)

    The format used for the texture view. 

* [u32 mip_slice](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1a6d27e4a4383c82f0fd25d296517f3b8b.md)

    The mip slice used for the texture view. 

* [u32 array_slice](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment_1af0b0cad0aa42b5145951ecd38a2d88ee.md)

    The array slice used for the texture view. 

