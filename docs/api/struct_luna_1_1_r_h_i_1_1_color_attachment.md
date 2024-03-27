# Luna::RHI::ColorAttachment
Describes one color attachment when beginning a render pass. 

```c++
struct Luna::RHI::ColorAttachment
```

## Member objects
* [ITexture* texture](struct_luna_1_1_r_h_i_1_1_color_attachment_1ab02abc67d0395436de0c53aca08fd08f.md)

    The texture to bind for this attachment. The texture must have [TextureUsageFlag::color_attachment](group___r_h_i_1gga158288d119b258c9a2dc7c2ca0cd2501a53e7889711e460d08eca0e6e3579951f.md) being set. 

* [LoadOp load_op](struct_luna_1_1_r_h_i_1_1_color_attachment_1aaeca1459065fbade2beb5a25615e0100.md)

    The load operation to perform when reading data from attachment. 

* [StoreOp store_op](struct_luna_1_1_r_h_i_1_1_color_attachment_1a15371cc3592a9b913ad8299442e59a9e.md)

    The store operation to perform when writing data to attachment. 

* [Float4U clear_value](struct_luna_1_1_r_h_i_1_1_color_attachment_1a14376be4217e7f35e9ea45a686ee7956.md)

    The clear value to use if `load_op` is [LoadOp::clear](group___r_h_i_1gga8d353cef0bd83ad8a6b73532498b26eea01bc6f8efa4202821e95f4fdf6298b30.md). Otherwise this value is ignored. 

* [TextureViewType view_type](struct_luna_1_1_r_h_i_1_1_color_attachment_1acd11f9e113324f80f5cdfc92570490e9.md)

    The texture view type to view the texture as an attachment. If [TextureViewType::unspecified](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9ad415f0e30c471dfdd9bc4f827329ef48.md) is set, the system loads the texture's texture type as view type. 

* [Format format](struct_luna_1_1_r_h_i_1_1_color_attachment_1a751c4987b2c6908c70a915ab18d36653.md)

    The format used for the texture view. 

* [u32 mip_slice](struct_luna_1_1_r_h_i_1_1_color_attachment_1a6d27e4a4383c82f0fd25d296517f3b8b.md)

    The mip slice used for the texture view. 

* [u32 array_slice](struct_luna_1_1_r_h_i_1_1_color_attachment_1af0b0cad0aa42b5145951ecd38a2d88ee.md)

    The array slice used for the texture view. 

