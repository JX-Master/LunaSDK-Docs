# Luna::RHI::DescriptorSetLayoutBinding
Describes one binding in one descriptor set. 

```c++
struct Luna::RHI::DescriptorSetLayoutBinding
```

## Member objects
* [u32 binding_slot](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_binding_1a8538e2a39a5897f354604c212f7c86bd.md)

    The slot to bind the descriptor(s). If `num_descs` is greater than 1, slots [binding_slot, binding_slot + num_descs) will be occupied and cannot be used in another bindings. The binding slot does not need to be continuous. 

* [u32 num_descs](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_binding_1a75011aed416db915a0af6d8d108cb95c.md)

    The number of descriptors for this binding. If this number is greater than 1, this binding will be interprated as one array of descriptors. If this is a variable-sized descriptors array, this is the maximum number of descriptors that may be bound. This value may be used for hardware validation when needed. 

* [DescriptorType type](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_binding_1a05248a33688a88a6e8f8a03c729e308e.md)

    The type of descriptors. 

* [TextureViewType texture_view_type](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_binding_1addb5069baf09736b65191acaf394264c.md)

    The type of the texture view if this binding represents one texture, otherwise [TextureViewType::unspecified](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9ad415f0e30c471dfdd9bc4f827329ef48.md). 

* [ShaderVisibilityFlag shader_visibility_flags](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_binding_1a41309789ee52bc3f6caecfe925048c2b.md)

    Specify which pipeline shader can access a resource for this binding. 

