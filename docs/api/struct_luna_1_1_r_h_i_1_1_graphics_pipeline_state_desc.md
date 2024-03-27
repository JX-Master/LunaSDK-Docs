# Luna::RHI::GraphicsPipelineStateDesc
Describes pipeline configurations of one compute pipeline. 

```c++
struct Luna::RHI::GraphicsPipelineStateDesc
```

## Member objects
* [InputLayoutDesc input_layout](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1ade6d847bab5734b0d2a503f11a703522.md)

    The input layout configurations. 

* [IPipelineLayout* pipeline_layout](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1af0b83f820d5368fea33d4fb6fa82f985.md)

    The compatible pipeline layout configurations. 

* [ShaderData vs](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a0bdc4d127c529336ebd6f5a397994c91.md)

    The vertex shader data. 

* [ShaderData ps](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a7edea5da5a5839eb81184c8cf39454f5.md)

    The pixel shader data. 

* [RasterizerDesc rasterizer_state](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a5cc87b28c29446d07d179b04fecb8fc4.md)

    The rasterizer configurations. 

* [DepthStencilDesc depth_stencil_state](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a0ca1c75a032d8ceaf2c6e1e967c3cb4a.md)

    The configurations of depth stencil stage. 

* [BlendDesc blend_state](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a409feb71c22ad837b94dfef618591f4f.md)

    The configurations of blend stage. 

* [IndexBufferStripCutValue ib_strip_cut_value](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a7a64f82954f7b3471888e96cec3a0efc.md)

    The index buffer strip cut value. This must match the format of the index buffer, see [IndexBufferStripCutValue](group___r_h_i_1ga63497036099cee50e2a03d13bbda77f1.md) for details. 

* [PrimitiveTopology primitive_topology](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1ad17233c42429f8e9367f7b3b29e2e98a.md)

    The primitive topology of primitives to be drawn. 

* [u8 num_color_attachments](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a2f368d307f2ab8738cbd343fe39cb9fd.md)

    The number of attachments that can be set. This must be a value between [`1`, `8`]. 

* [Format color_formats[8]](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1ac4eeae32d54c57f56f94a917e49263a4.md)

    The color attachment formats. Only [`0`, `num_color_attachments`) elements in this array will be used, other elements will be ignored. 

* [Format depth_stencil_format](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a2b45f5c9f8ffe247c026944eb920d3c5.md)

    The depth stencil attachment format. This must be Format::unknown if depth stencil attachment is not used. 

* [u32 sample_count](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1a1c8270d54620086aa497d8d7ee065458.md)

    Specify the sample count. This must be `1` if MSAA is not used. 

