# Luna::RHI::DescriptorSetLayoutBinding::binding_slot

```c++
u32 binding_slot
```

The slot to bind the descriptor(s). If `num_descs` is greater than 1, slots [binding_slot, binding_slot + num_descs) will be occupied and cannot be used in another bindings. The binding slot does not need to be continuous. 

