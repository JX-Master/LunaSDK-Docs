# Luna::RHI::ICommandBuffer::begin_render_pass

```c++
virtual void begin_render_pass(const RenderPassDesc &desc)=0
```

Starts a new render pass. The previous render pass should be closed before beginning another one. 



## Parameters
* *in* **desc**

    The render pass descriptor object.


The following functions can only be called in between [begin_render_pass](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1aa99d1993aba087706af06f8b5d00ec3e.md) and end_render_pass:* set_graphics_pipeline_layout

* set_graphics_pipeline_state

* set_vertex_buffers

* set_index_buffer

* set_graphics_descriptor_set

* set_graphics_descriptor_sets

* set_viewport

* set_viewports

* set_scissor_rect

* set_scissor_rects

* set_blend_factor

* set_stencil_ref

* draw

* draw_indexed

* draw_instanced

* draw_indexed_instanced

* clear_color_attachment

* clear_depth_stencil_attachment

The following functions can only be called outside of one render pass range:* submit

* set_context

* resource_barrier 

