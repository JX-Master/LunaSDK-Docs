# Luna::RHI::WriteDescriptorSet::buffer_views

```c++
const BufferViewDesc* buffer_views
```

The pointer to buffer view descriptors data array to be written. This array must have at least `num_descs` elements, and will be used if `type` is [DescriptorType::uniform_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a34a06ac1c4c09077554ac744585760a8.md), [DescriptorType::read_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a6a92853feaf697b82bc7a540363df626.md) or [DescriptorType::read_write_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2ac803981c38618413594fc9655c788c01.md). 

