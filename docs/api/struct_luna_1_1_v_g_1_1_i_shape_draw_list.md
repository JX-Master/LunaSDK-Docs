# Luna::VG::IShapeDrawList
Represents a draw list that contains shapes to be drawn. 

```c++
struct Luna::VG::IShapeDrawList : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual void reset()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a20dcbdfbd0ec77afc802522bb7e379c1.md)

    Resets the draw list. The call clears all shapes recorded, but retains their memory and resources, so they can be reused for new shapes. 

* [virtual void set_shape_buffer(RHI::IBuffer *shape_buffer)=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1aba5d1ef7334f2555f74e5f07233b225f.md)

    Sets the shape buffer used for the following draw calls. 

* [virtual RHI::IBuffer * get_shape_buffer()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1af4ca44bdf13d520ea614864492056e35.md)

    Gets the current shape buffer. 

* [virtual void set_texture(RHI::ITexture *tex)=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a1762e6f0783e2c18689976d786dcf3fb.md)

    Sets the texture to be sampled when rendering the succeeding shapes. 

* [virtual RHI::ITexture * get_texture()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a12ee819125d39131821d2668597e4d79.md)

    Gets the currently set texture, returns `nullptr` if no texture is set. 

* [virtual void set_sampler(const RHI::SamplerDesc *desc)=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1ae6fe6eeb0c09bc330aa1c631560b615f.md)

    Sets the sampler state to be used when sampling bound textures. Specify `nullptr` to reset the sampler state to initial settings. 

* [virtual RHI::SamplerDesc get_sampler()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a714f8688782995fa6d0046e82126f8af.md)

    Gets the sampler state currently set. 

* [virtual void set_origin(const Float2 &origin)=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a0b35020bfb0e9efa0e1648d7abef3aba.md)

    Sets the origin point for the following draw calls. The origin point is relative to the origin point of the canvas. The origin point of the canvas is at the bottom-left corner. The x axis points to right and the y axis points to up. 

* [virtual Float2 get_origin()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1aeb5744facdc937d5e72f4a5093c31fcc.md)

    Gets the origin point for the following draw calls. 

* [virtual void set_rotation(f32 degrees)=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a03aaf7fb0ccfd118320954b24fa4c8e0.md)

    Sets the rotation for the following draw calls, the rotation is relative to the set origin point. The rotation is specified in clockwise degrees. 

* [virtual f32 get_rotation()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a8e0226d1ee276ca89e8fb296169dca08.md)

    Gets the rotation for the following draw calls. 

* [virtual void draw_shape_raw(Span< const Vertex > vertices, Span< const u32 > indices)=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a4ac15584de4038588b4f4561e74303e3.md)

    Draws one shape by submitting vertices and indices directly. 

* [virtual void draw_shape(u32 begin_command, u32 num_commands, const Float2U &min_position, const Float2U &max_position, const Float2U &min_shapecoord, const Float2U &max_shapecoord, u32 color=0xFFFFFFFF, const Float2U &min_texcoord=Float2U(0.0f), const Float2U &max_texcoord=Float2U(0.0f))=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a035af2fc2d301283064df927cec46882.md)

    Draws one shape. The shape is drawn by adding one draw rect (two triangles) to the list. 

* [virtual RV close()=0](struct_luna_1_1_v_g_1_1_i_shape_draw_list_1a2ab4c2a45b005f0fb5d3d01ae76ea35f.md)

    Finishes the shape recording and generates draw calls that can be passed to RHI. 

