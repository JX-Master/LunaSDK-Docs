# Luna::RHI::DescriptorSetLayoutBinding::num_descs

```c++
u32 num_descs
```

The number of descriptors for this binding. If this number is greater than 1, this binding will be interprated as one array of descriptors. If this is a variable-sized descriptors array, this is the maximum number of descriptors that may be bound. This value may be used for hardware validation when needed. 

