# Luna::RHI::ICommandBuffer::set_graphics_descriptor_set

```c++
virtual void set_graphics_descriptor_set(u32 index, IDescriptorSet *descriptor_set)=0
```

Sets the descriptor set to be used by the graphic pipeline. 

This behaves the same as calling [set_graphics_descriptor_sets](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a8000f3cf88cafdb071339a25e5b7599a.md) with only one element. 

## Parameters
* *in* **index**

    The binding index of the descriptor set. This must be smaller than the size of [PipelineLayoutDesc::descriptor_set_layouts](struct_luna_1_1_r_h_i_1_1_pipeline_layout_desc_1af14fb6495cacbbf8522b496fd1681901.md) of the binding pipeline layout. 

* *in* **descriptor_set**

    The descriptor set to set. 

## Valid Usage
* This must be called after [set_graphics_pipeline_state](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a74cc0f93a3aa327e788789b87a5cd891.md) and [set_graphics_pipeline_layout](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a35de6b8341e6e61c170167b32f9ddf41.md). 

