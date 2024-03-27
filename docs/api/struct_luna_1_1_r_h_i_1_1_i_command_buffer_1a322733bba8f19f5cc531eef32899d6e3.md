# Luna::RHI::ICommandBuffer::set_compute_descriptor_set

```c++
virtual void set_compute_descriptor_set(u32 index, IDescriptorSet *descriptor_set)=0
```

Sets the descriptor set to be used by the compute pipeline. 

This behaves the same as calling set_computes_descriptor_sets with only one element. 

## Parameters
* *in* **index**

    The binding index of the descriptor set. This must be smaller than the size of [PipelineLayoutDesc::descriptor_set_layouts](struct_luna_1_1_r_h_i_1_1_pipeline_layout_desc_1af14fb6495cacbbf8522b496fd1681901.md) of the binding pipeline layout. 

* *in* **descriptor_set**

    The descriptor set to set. 

## Valid Usage
* This must be called after set_computes_pipeline_state and set_computes_pipeline_layout. 

