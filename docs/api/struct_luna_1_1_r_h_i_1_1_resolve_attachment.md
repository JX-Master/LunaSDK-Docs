# Luna::RHI::ResolveAttachment
Describes one resolve attachment when beginning a render pass. 

```c++
struct Luna::RHI::ResolveAttachment
```

A resolve attachment is used to resolve data in one MSAA texture into one normal texture. 

## Member objects
* [ITexture* texture](struct_luna_1_1_r_h_i_1_1_resolve_attachment_1ab02abc67d0395436de0c53aca08fd08f.md)

    The texture to bind for this attachment. This texture is used as resolve target. The texture must have [TextureUsageFlag::resolve_attachment](group___r_h_i_1gga158288d119b258c9a2dc7c2ca0cd2501ab766f6724ffd961503585768223f66f6.md) being set. 

* [u32 mip_slice](struct_luna_1_1_r_h_i_1_1_resolve_attachment_1a6d27e4a4383c82f0fd25d296517f3b8b.md)

    The mip slice used for the texture view. 

* [u32 array_slice](struct_luna_1_1_r_h_i_1_1_resolve_attachment_1af0b0cad0aa42b5145951ecd38a2d88ee.md)

    The first slice in the texture view. 

* [u32 array_size](struct_luna_1_1_r_h_i_1_1_resolve_attachment_1acdbb4e4a711c816c1e63fcb9ece8f73c.md)

    The number of array elements in the texture view, range in [array_slice, array_slice + array_size). 

