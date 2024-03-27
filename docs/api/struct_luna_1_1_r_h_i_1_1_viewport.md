# Luna::RHI::Viewport
Describes one viewport used by [ICommandBuffer::set_viewport](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ade5bc1a0f452cc3e355040ae00499efb.md) and [ICommandBuffer::set_viewports](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abe3f9b469aa3574cd81974f7523f9cac.md). 

```c++
struct Luna::RHI::Viewport
```

## Member objects
* [f32 top_left_x](struct_luna_1_1_r_h_i_1_1_viewport_1a84766513882b39c8834b82e7f680ffb6.md)

    The X position, in pixels, of the top left corner of the viewport, relative to the top left corner of the render target (X axis points to right). 

* [f32 top_left_y](struct_luna_1_1_r_h_i_1_1_viewport_1a452af4ddbd6dee8db1bd47be3e161b66.md)

    The Y position, in pixels, of the top left corner of the viewport, relative to the top left corner of the render target (Y axis points to down). 

* [f32 width](struct_luna_1_1_r_h_i_1_1_viewport_1aa679a70417d68bf8a6321393fc8904d9.md)

    The width of the viewport in pixels. 

* [f32 height](struct_luna_1_1_r_h_i_1_1_viewport_1a4b7abb62d44402da79ba4821606262bd.md)

    The height of the viewport in pixels. 

* [f32 min_depth](struct_luna_1_1_r_h_i_1_1_viewport_1a042763a0d664a9c1b714db67d5db97f2.md)

    The minimum depth value of the viewport. The value must between [0.0, 1.0]. 

* [f32 max_depth](struct_luna_1_1_r_h_i_1_1_viewport_1a3c9097fee754e33c58e30a2d115cae4d.md)

    The maximum depth value of the viewport. The value must between [0.0, 1.0]. 

