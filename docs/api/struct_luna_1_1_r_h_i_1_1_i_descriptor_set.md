# Luna::RHI::IDescriptorSet
Describes which views and samples are bound to the pipeline. This can be set at any time before the draw call or dispatch call is submitted. 

```c++
interface Luna::RHI::IDescriptorSet : public virtual IDeviceChild
```

## Base type
* [IDeviceChild](struct_luna_1_1_r_h_i_1_1_i_device_child.md)
## Member functions
* [virtual RV update_descriptors(Span< const WriteDescriptorSet > writes)=0](struct_luna_1_1_r_h_i_1_1_i_descriptor_set_1a6431c1c91d34b06fab9ca589d58a7150.md)

    Updates descriptors' data in this descriptor set. 

