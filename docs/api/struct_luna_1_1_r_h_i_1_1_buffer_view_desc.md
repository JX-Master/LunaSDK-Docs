# Luna::RHI::BufferViewDesc
Describes one buffer view in descriptor set. 

```c++
struct Luna::RHI::BufferViewDesc
```

## Member objects
* [u64 first_element](struct_luna_1_1_r_h_i_1_1_buffer_view_desc_1ac6ee3dd2a92551758d3a3eaa1ecc2d23.md)

    If this is a uniform buffer, specify the offset, in bytes, of the data to be viewed. If this is a structured buffer, specify the index of the first element to be accessed by the view. 

* [IBuffer* buffer](struct_luna_1_1_r_h_i_1_1_buffer_view_desc_1a66b6e32a2ca728d104d46a04a74e4f09.md)

    The buffer to set. 

* [u32 element_count](struct_luna_1_1_r_h_i_1_1_buffer_view_desc_1a1657d38ebdc743039294507f0a4c4eda.md)

    The number of elements in this view. This must be set to 1 if this is a uniform buffer view. 

* [u32 element_size](struct_luna_1_1_r_h_i_1_1_buffer_view_desc_1a36f30ec6d16cb21f6e95ec28326a6809.md)

    If this is a uniform buffer, specify the size, in bytes, of the uniform buffer. If this is a structured buffer, specify the size, in bytes, of each element in the buffer structure. 

