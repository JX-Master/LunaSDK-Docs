# Luna::VG::Vertex
Describes one vertex to be drawn for the glyph. 

```c++
struct Luna::VG::Vertex
```

## Member objects
* [Float2U position](struct_luna_1_1_v_g_1_1_vertex_1a41b056d44061892a4fd23b9415db09ea.md)

    The position of the vertex. 

* [Float2U shapecoord](struct_luna_1_1_v_g_1_1_vertex_1aea6ba3a131899e37951c582e2b3f3414.md)

    The shape coordinate of the vertex for mapping the shape commands. 

* [Float2U texcoord](struct_luna_1_1_v_g_1_1_vertex_1a6f75cca9f17ee22f7a498867ee47d6f9.md)

    The texture coordinate of the vertex for sampling the attached resources. 

* [u32 color](struct_luna_1_1_v_g_1_1_vertex_1a5e38aaa680835a5c432886bd64e55bb6.md)

    An additional color that can be used to tint the vertex. 

* [u32 begin_command](struct_luna_1_1_v_g_1_1_vertex_1a1ffb01e26ec634d5dc32381facbdcb1d.md)

    The offset of the first command for this shape in the shape buffer. 

* [u32 num_commands](struct_luna_1_1_v_g_1_1_vertex_1af906c08de26e0accce816e07404ca8ff.md)

    The number of commands (f32 values) used for this shape. 

