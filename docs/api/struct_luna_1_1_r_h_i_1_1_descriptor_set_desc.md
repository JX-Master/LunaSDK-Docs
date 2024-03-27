# Luna::RHI::DescriptorSetDesc
Describes one descriptor set. 

```c++
struct Luna::RHI::DescriptorSetDesc
```

## Member objects
* [IDescriptorSetLayout* layout](struct_luna_1_1_r_h_i_1_1_descriptor_set_desc_1ac7acefdc4d0f2454dd42ddc8dbd90e92.md)

    The descriptor layout for this descriptor set. 

* [u32 num_variable_descriptors](struct_luna_1_1_r_h_i_1_1_descriptor_set_desc_1aad00d299621f7512f8192a7066e3c96d.md)

    If the descriptor layout has `DescriptorSetLayoutFlag::variable_descriptors` set, this is the number of variable descriptors being allocated for this else. Otherwise, this should always be 0. 

