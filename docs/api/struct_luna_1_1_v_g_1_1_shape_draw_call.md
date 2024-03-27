# Luna::VG::ShapeDrawCall
Describes one shape draw call. 

```c++
struct Luna::VG::ShapeDrawCall
```

## Member objects
* [RHI::IBuffer* shape_buffer](struct_luna_1_1_v_g_1_1_shape_draw_call_1ae2248423dc8961e0c1e6276610318ef2.md)

    The shape buffer bind to this draw call. 

* [RHI::ITexture* texture](struct_luna_1_1_v_g_1_1_shape_draw_call_1a71147d494da540fce9c3b44cfd55157a.md)

    The texture bind to this draw call. May be `nullptr`. 

* [RHI::SamplerDesc sampler](struct_luna_1_1_v_g_1_1_shape_draw_call_1a123d16efcaaa17b18a110075b40e8f25.md)

    The attached sampler for this draw call. 

* [u32 base_index](struct_luna_1_1_v_g_1_1_shape_draw_call_1a4f526461b30ecc4d210b19397876b486.md)

    The fist index to draw for this draw call. 

* [u32 num_indices](struct_luna_1_1_v_g_1_1_shape_draw_call_1ad729b2960d6270018851f526c3f32637.md)

    The number of indices to draw for this draw call. 

* [Float2U origin_point](struct_luna_1_1_v_g_1_1_shape_draw_call_1a87cc51ea9e668b056b56b72322671f08.md)

    The origin point for this draw call. 

* [f32 rotation](struct_luna_1_1_v_g_1_1_shape_draw_call_1a347c5138b505c66ec009ce742a41b980.md)

    The rotation for this draw call. 

