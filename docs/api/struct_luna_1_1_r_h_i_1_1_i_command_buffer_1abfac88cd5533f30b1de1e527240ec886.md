# Luna::RHI::ICommandBuffer::set_scissor_rect

```c++
virtual void set_scissor_rect(const RectI &rect)=0
```

Binds one scissor rectangle to the rasterizer stage. The scissor rectangle points are relative to the top-left corner of the render target, with x-axis points to right and y-axis points to down. 

This operation behaves the same as calling [set_scissor_rects](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a33287fd90025df885a4703c4796dd0e5.md) with only one scissor rect. 

## Parameters
* *in* **rect**

    The scissor rectangle to set. 

