# Luna::RHI::DepthStencilDesc
Describes depth stencil stage configurations of one graphics pipeline. 

```c++
struct Luna::RHI::DepthStencilDesc
```

## Member objects
* [bool depth_test_enable](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1ac0c9fb6e160609c188cd8086edb1d880.md)

    Whether depth testing is enabled. If this is `false`, all pixels from pixel shader will pass depth testing. 

* [bool depth_write_enable](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1a1f3cd71663241d9459373b82ab4edeb3.md)

    Whether to write the pixel's depth value to depth buffer if one pixel passes depth testing. 

* [CompareFunction depth_func](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1aeaf81f81b30ad27f1583c5097f5b6f1a.md)

    The compare function used for depth comparison in depth testing. 

* [bool stencil_enable](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1a1bbf1b2df0c5ef608d5710db9b86bcf5.md)

    Whether stencil testing is enabled. If this is `false`, all pixels from pixel shader will pass stencil testing. 

* [u8 stencil_read_mask](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1a54fc9dd9e4aedfe7ae7f3240cb29a072.md)

    The mask used to specify bits that will be loaded from stencil buffer for stencil testing. All bits that are not specified in the mask (with mask bit value 0) will be set to 0 before stencil testing is performed. 

* [u8 stencil_write_mask](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1a0b75ffe65e2544a378f77ca9582bbdf5.md)

    The mask used to specify bits that are allowed to be modified in stencil testing. 

* [DepthStencilOpDesc front_face](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1a1cbb4d2784fd024910ca52c3701ce9ae.md)

    The depth stencil operation performed for the front face of one triangle. 

* [DepthStencilOpDesc back_face](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc_1a06707b85ef4a85b88f6bef737c74b0a7.md)

    The depth stencil operation performed for the back face of one triangle. 

