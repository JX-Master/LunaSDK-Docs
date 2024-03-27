# Luna::RHI::ICommandBuffer::set_graphics_descriptor_sets

```c++
virtual void set_graphics_descriptor_sets(u32 start_index, Span< IDescriptorSet * > descriptor_sets)=0
```

Sets descriptor sets to be used by the graphic pipeline. 



## Parameters
* *in* **start_index**

    The binding index of the first descriptor set in the array. Descriptor sets in the array will be bound in range [`start_index`, `start_index + descriptor_sets.size()`). 

* *in* **descriptor_sets**

    The descriptor sets to set. 

## Valid Usage
* This must be called after [set_graphics_pipeline_state](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a74cc0f93a3aa327e788789b87a5cd891.md) and [set_graphics_pipeline_layout](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a35de6b8341e6e61c170167b32f9ddf41.md). 

