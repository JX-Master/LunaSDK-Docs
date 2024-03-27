# Luna::RHI::WriteDescriptorSet
Describes one descriptor set write operation. Every descriptor set write operation may update one continuous range of descriptors in the same binding slot. 

```c++
struct Luna::RHI::WriteDescriptorSet
```

## Member objects
* [u32 binding_slot](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1a8538e2a39a5897f354604c212f7c86bd.md)

    The binding slot of the descriptors to update. 

* [u32 first_array_index](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1ad637c6f2456917210f082f421d965e8e.md)

    The slot offset of the first descriptor to update relative to the binding slot. 

* [u32 num_descs](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1a75011aed416db915a0af6d8d108cb95c.md)

    The number of descriptors to write. 

* [DescriptorType type](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1a05248a33688a88a6e8f8a03c729e308e.md)

    The type of the descriptors to write. This must be equal to the actual type of the descriptors in the descriptor array. 

* [const BufferViewDesc* buffer_views](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1ab8dbdc5f22aa7995b85df22e6ab1458f.md)

    The pointer to buffer view descriptors data array to be written. This array must have at least `num_descs` elements, and will be used if `type` is [DescriptorType::uniform_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a34a06ac1c4c09077554ac744585760a8.md), [DescriptorType::read_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a6a92853feaf697b82bc7a540363df626.md) or [DescriptorType::read_write_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2ac803981c38618413594fc9655c788c01.md). 

* [const TextureViewDesc* texture_views](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1ab17c8f4b2a81bc5877c8be3993791c8c.md)

    The pointer to texture view descriptors data array to be written. This array must have at least `num_descs` elements, and will be used if `type` is [DescriptorType::read_texture_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2aceda36ce0ea7592cd04d237493431753.md) and [DescriptorType::read_write_texture_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2aff0f72f27c8460d323630827e870a1ba.md). 

* [const SamplerDesc* samplers](struct_luna_1_1_r_h_i_1_1_write_descriptor_set_1a5e3e50e6770c0691af10310617a6102f.md)

    The pointer to sampler descriptors data array to be written. This array must have at least `num_descs` elements, and will be used if `type` is [DescriptorType::sampler](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a2b06a2251d39e28f8220696766dcd136.md). 

