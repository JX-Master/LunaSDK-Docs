# Luna::RHI::ICommandBuffer::set_compute_descriptor_sets

```c++
virtual void set_compute_descriptor_sets(u32 start_index, Span< IDescriptorSet * > descriptor_sets)=0
```

Sets descriptor sets to be used by the compute pipeline. 



## Parameters
* *in* **start_index**

    The binding index of the first descriptor set in the array. Descriptor sets in the array will be bound in range [`start_index`, `start_index + descriptor_sets.size()`). 

* *in* **descriptor_sets**

    The descriptor sets to set. 

## Valid Usage
* This must be called after set_computes_pipeline_state and set_computes_pipeline_layout. 

