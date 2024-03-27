# Luna::RHI::ICommandBuffer::set_viewports

```c++
virtual void set_viewports(Span< const Viewport > viewports)=0
```

Bind an array of viewports to the rasterizer stage of the pipeline. 

All viewports must be set in one call. Any call to [set_viewport](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ade5bc1a0f452cc3e355040ae00499efb.md) or [set_viewports](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abe3f9b469aa3574cd81974f7523f9cac.md) clears all existing viewports before setting new viewports. 

