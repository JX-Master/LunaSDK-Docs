# Luna::RHI::InputAttributeDesc
Describes one attribute in the input layout. 

```c++
struct Luna::RHI::InputAttributeDesc
```

## Member objects
* [const c8* semantic_name](struct_luna_1_1_r_h_i_1_1_input_attribute_desc_1a8a5cfae87e5ce9d30d930cd9431c7ffc.md)

    The semantic name of this attribute. For exmaple, "COLOR", "TEXCOORD", etc. 

* [u32 semantic_index](struct_luna_1_1_r_h_i_1_1_input_attribute_desc_1aa9f35647eb7afef14ab8f6c81e6b0809.md)

    The semantic index of this attribute. Use this to differentiate attributes with the same semantic name. 

* [u32 location](struct_luna_1_1_r_h_i_1_1_input_attribute_desc_1a4a9ba2d08e8c8b11eece7c1d7e2fb28e.md)

    The location of this input attribute in the shader. 

* [u32 binding_slot](struct_luna_1_1_r_h_i_1_1_input_attribute_desc_1a8538e2a39a5897f354604c212f7c86bd.md)

    The belonging binding slot of this attribute. 

* [u32 offset](struct_luna_1_1_r_h_i_1_1_input_attribute_desc_1a4ba37e6b40e12ce1d1e5dbee0323069d.md)

    The offset of this attribute from the beginning of the element. 

* [Format format](struct_luna_1_1_r_h_i_1_1_input_attribute_desc_1a751c4987b2c6908c70a915ab18d36653.md)

    The format of this attribute. 

