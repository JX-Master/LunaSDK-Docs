# Luna::RHI::VertexBufferView
Describes one vertex buffer view when binding one vertex buffer to the render pipeline. 

```c++
struct Luna::RHI::VertexBufferView
```

## Member objects
* [IResource* buffer](struct_luna_1_1_r_h_i_1_1_vertex_buffer_view_1a4be656082bc4454c545d83e07fe4623c.md)

    The vertex buffer resource. 

* [usize offset](struct_luna_1_1_r_h_i_1_1_vertex_buffer_view_1af54fc49734a070e8a5568b09bb23a9d5.md)

    The offset, in bytes, of the first vertex from the beginning of the buffer. 

* [u32 size](struct_luna_1_1_r_h_i_1_1_vertex_buffer_view_1acfd6273064c5acdcfc39a23a69dd4343.md)

    The size, in bytes, of the vertex buffer range to bind. 

* [u32 element_size](struct_luna_1_1_r_h_i_1_1_vertex_buffer_view_1a36f30ec6d16cb21f6e95ec28326a6809.md)

    The size, in butes, of every vertex element in the vertex buffer. The element size must be equal to `InputBindingDesc::element_size` of the pipeline state object used to draw this vertex buffer. 

