# Luna::RHI::ICommandBuffer::set_scissor_rects

```c++
virtual void set_scissor_rects(Span< const RectI > rects)=0
```

Binds an array of scissor rectangles to the rasterizer stage. The scissor rectangle points are relative to the top-left corner of the render target, with x-axis points to right and y-axis points to down. 

All scissor rectangles must be set in one call. Any call to [set_scissor_rect](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abfac88cd5533f30b1de1e527240ec886.md) or [set_scissor_rects](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a33287fd90025df885a4703c4796dd0e5.md) clears all existing scissor rectangles before setting new scissor rectangles. 

## Parameters
* *in* **rects**

    The scissor rectangles to set. 

