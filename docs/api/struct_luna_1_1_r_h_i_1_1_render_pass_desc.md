# Luna::RHI::RenderPassDesc
Describes one render pass. 

```c++
struct Luna::RHI::RenderPassDesc
```

## Member objects
* [ColorAttachment color_attachments[8]](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1a01b3edfee2e9159bc4e60cefe47f156d.md)

    The color attachments to set. 

* [ResolveAttachment resolve_attachments[8]](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1a73a66bc0f6690718651e0fd15f564695.md)

    The resolve attachments to set. 

* [DepthStencilAttachment depth_stencil_attachment](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1acab1761cc576caca240185f4745745f7.md)

    The depth stencil attachment to set. 

* [IQueryHeap* occlusion_query_heap](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1aa307149bdc7aa7a50da9ad2a84931830.md)

    The occlustion query heap that the query data will be written to if not `nullptr`. 

* [IQueryHeap* timestamp_query_heap](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1ad8f257d32b9f8609cae0973c09b61dfc.md)

    The timestamp query heap that the query data will be written to if not `nullptr`. 

* [IQueryHeap* pipeline_statistics_query_heap](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1af73b3b78911a849e97de8795f33476a3.md)

    The pipeline statistics query heap that the query data will be written to if not `nullptr`. 

* [u32 timestamp_query_begin_pass_write_index](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1abdce645223cefbb19c950af746cbd2eb.md)

    The index of the element in timestamp query heap that the render pass begin timestamp will be written to. If this is [DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md), the query data will not be written. 

* [u32 timestamp_query_end_pass_write_index](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1a8852fe8f6016604273236959c8f2af78.md)

    The index of the element in timestamp query heap that the render pass end timestamp will be written to. If this is [DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md), the query data will not be written. 

* [u32 pipeline_statistics_query_write_index](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1aab659b8951b9eea11f8ec237e202aaf1.md)

    The index of the element in pipeline statistics query heap that the pipeline statistics will be written to. If this is [DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md), the query data will not be written. 

* [u32 array_size](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1acdbb4e4a711c816c1e63fcb9ece8f73c.md)

    The number of texture array elements that will be bound for all attachments. 

* [u8 sample_count](struct_luna_1_1_r_h_i_1_1_render_pass_desc_1a344a0db2b0250fb750c41b09a5b2c02c.md)

    The sample count for every pixel of the render pass. Specify any value greater than 1 enables MSAA. 

