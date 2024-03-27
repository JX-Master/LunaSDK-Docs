# Luna::RHI::ICommandBuffer
Used to allocate memory for commands, record commands, submitting commands to GPU and tracks the state of the submitted commands. 

```c++
interface Luna::RHI::ICommandBuffer : public virtual IDeviceChild, public virtual IWaitable
```

Command buffer is not thread safe. If the user need to record commands simultaneously, she should create multiple command buffers, one per thread.

All synchroizations for command buffers are performed explicitly, for instance:1. Use [ICommandBuffer::wait](struct_luna_1_1_i_waitable_1a0c78500b6312f13b1d666b30b40fe132.md) to wait for one command buffer from host side,

1. Use fence objects to wait for one command buffer from another command buffer.

1. Only call [ICommandBuffer::reset](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a39612d7442b0dc582b84e15c940c52a3.md) after the command buffer is not submitted, or is finished by GPU. 

## Base types
* [IDeviceChild](struct_luna_1_1_r_h_i_1_1_i_device_child.md)
* [IWaitable](struct_luna_1_1_i_waitable.md)
## Member functions
* [virtual u32 get_command_queue_index()=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a9834224add57a79eb4f28dc3ed21f144.md)

    Gets the command queue index of the command queue attached to this buffer. 

* [virtual RV reset()=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a39612d7442b0dc582b84e15c940c52a3.md)

    Resets the command buffer. This call clears all commands in the command buffer, resets the state tracking infrastructure and reopens the command buffer for recording new commands. 

* [virtual void attach_device_object(IDeviceChild *obj)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a8ccb3b5123e60da920f75df12fbfb75b.md)

    Attaches one graphic device object to this command buffer. The command buffer keeps a strong reference to the object until the next `reset` is called. 

* [virtual void begin_event(const c8 *event_name)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abed00e201a0ce30f29f4a42f8c70a370.md)

    Begins a new event. This is for use in diagnostic tools like RenderDoc, PIX, XCode, etc to group commands into hierarchical sections. 

* [virtual void end_event()=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abc429c8821b0ab21c07d872f6c6153e4.md)

    Ends the latest event opened by [begin_event](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abed00e201a0ce30f29f4a42f8c70a370.md) that has not been ended. 

* [virtual void begin_render_pass(const RenderPassDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1aa99d1993aba087706af06f8b5d00ec3e.md)

    Starts a new render pass. The previous render pass should be closed before beginning another one. 

* [virtual void set_graphics_pipeline_layout(IPipelineLayout *pipeline_layout)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a35de6b8341e6e61c170167b32f9ddf41.md)

    Sets the graphic pipeline layout. 

* [virtual void set_graphics_pipeline_state(IPipelineState *pso)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a74cc0f93a3aa327e788789b87a5cd891.md)

    Sets the pipeline state for graphics pipeline. 

* [virtual void set_vertex_buffers(u32 start_slot, Span< const VertexBufferView > views)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abc8909a35c19461cb87021c7e30be119.md)

    Sets vertex buffers. 

* [virtual void set_index_buffer(const IndexBufferView &view)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a2b2a8fb462f0d158279ea417ea652788.md)

    Sets the index buffer. 

* [virtual void set_graphics_descriptor_set(u32 index, IDescriptorSet *descriptor_set)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a816de9e5a70152f765bc0fe701024080.md)

    Sets the descriptor set to be used by the graphic pipeline. 

* [virtual void set_graphics_descriptor_sets(u32 start_index, Span< IDescriptorSet * > descriptor_sets)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a8000f3cf88cafdb071339a25e5b7599a.md)

    Sets descriptor sets to be used by the graphic pipeline. 

* [virtual void set_viewport(const Viewport &viewport)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ade5bc1a0f452cc3e355040ae00499efb.md)

    Bind one viewport to the rasterizer stage of the pipeline. 

* [virtual void set_viewports(Span< const Viewport > viewports)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abe3f9b469aa3574cd81974f7523f9cac.md)

    Bind an array of viewports to the rasterizer stage of the pipeline. 

* [virtual void set_scissor_rect(const RectI &rect)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abfac88cd5533f30b1de1e527240ec886.md)

    Binds one scissor rectangle to the rasterizer stage. The scissor rectangle points are relative to the top-left corner of the render target, with x-axis points to right and y-axis points to down. 

* [virtual void set_scissor_rects(Span< const RectI > rects)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a33287fd90025df885a4703c4796dd0e5.md)

    Binds an array of scissor rectangles to the rasterizer stage. The scissor rectangle points are relative to the top-left corner of the render target, with x-axis points to right and y-axis points to down. 

* [virtual void set_blend_factor(const Float4U &blend_factor)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1aff2ce4e90c11f489deb3c5f576693c95.md)

    Sets the blend factor of the graphics pipeline. 

* [virtual void set_stencil_ref(u32 stencil_ref)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a02299becd77ad76f7ce0e8ebf47003e1.md)

    Sets the reference value for stencil testing. 

* [virtual void draw(u32 vertex_count, u32 start_vertex_location)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a14dc3770ace9f0e4adff58d3e7d8ee02.md)

    Draw primitives. 

* [virtual void draw_indexed(u32 index_count, u32 start_index_location, i32 base_vertex_location)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ac3608cb85ce08de63a395cad0415b73e.md)

    Draw indexed primitives. 

* [virtual void draw_instanced(u32 vertex_count_per_instance, u32 instance_count, u32 start_vertex_location, u32 start_instance_location)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a4dba44f13cd55c94dda7a10cb77f7637.md)

    Draws non-indexed, instanced primitives. 

* [virtual void draw_indexed_instanced(u32 index_count_per_instance, u32 instance_count, u32 start_index_location, i32 base_vertex_location, u32 start_instance_location)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a1d4d8fef30b4a5e11139e95ebd34b2bc.md)

    Draws indexed, instanced primitives. 

* [virtual void begin_occlusion_query(OcclusionQueryMode mode, u32 index)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a8138cfa194c51252c1dd04887a492123.md)

    Starts one occlusion query. 

* [virtual void end_occlusion_query(u32 index)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a39d362d6941faec8bfd6a030d33b2089.md)

    Ends one existing occlusion query. 

* [virtual void end_render_pass()=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a47518c4983c197c3fcb31d9ef7581d26.md)

    Finishes the current render pass. 

* [virtual void begin_compute_pass(const ComputePassDesc &desc=ComputePassDesc())=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1aef457c1a4f3841c6444c5b53dc007810.md)

    Begins a compute pass. 

* [virtual void set_compute_pipeline_layout(IPipelineLayout *pipeline_layout)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a55bde8ff3196320c0c768da812a35950.md)

    Sets the compute pipeline layout. 

* [virtual void set_compute_pipeline_state(IPipelineState *pso)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a03ea4f33e0e8e1c5c8d420e552d0d367.md)

    Sets the pipeline state for compute pipeline. 

* [virtual void set_compute_descriptor_set(u32 index, IDescriptorSet *descriptor_set)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a322733bba8f19f5cc531eef32899d6e3.md)

    Sets the descriptor set to be used by the compute pipeline. 

* [virtual void set_compute_descriptor_sets(u32 start_index, Span< IDescriptorSet * > descriptor_sets)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1af6e005e8cca6f2fb0f77714edd6c694f.md)

    Sets descriptor sets to be used by the compute pipeline. 

* [virtual void dispatch(u32 thread_group_count_x, u32 thread_group_count_y, u32 thread_group_count_z)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a6653457de27dff92f18565e1790574fa.md)

    Dispatches one compute task. 

* [virtual void end_compute_pass()=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a232159132f7e1a0ae38f0c83744a7b98.md)

    Ends a compute pass. 

* [virtual void begin_copy_pass(const CopyPassDesc &desc=CopyPassDesc())=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ab3e6055cc4974cb38dcd2ce5fba1c1de.md)

    Begins a copy pass. 

* [virtual void copy_resource(IResource *dst, IResource *src)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a379b1be5ee3eeaa3fdf88da8e2a8a99b.md)

    Copies the entire contents of the source resource to the destination resource. 

* [virtual void copy_buffer(IBuffer *dst, u64 dst_offset, IBuffer *src, u64 src_offset, u64 copy_bytes)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a3967f43bb0f7dabd56a3c12697b00316.md)

    Copies buffer data region from one buffer to another. 

* [virtual void copy_texture(ITexture *dst, SubresourceIndex dst_subresource, u32 dst_x, u32 dst_y, u32 dst_z, ITexture *src, SubresourceIndex src_subresource, u32 src_x, u32 src_y, u32 src_z, u32 copy_width, u32 copy_height, u32 copy_depth)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a918d6b71f069fb7abfe41d5e32442b29.md)

    Copies texture data region from one texture to another. 

* [virtual void copy_buffer_to_texture(ITexture *dst, SubresourceIndex dst_subresource, u32 dst_x, u32 dst_y, u32 dst_z, IBuffer *src, u64 src_offset, u32 src_row_pitch, u32 src_slice_pitch, u32 copy_width, u32 copy_height, u32 copy_depth)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a4bae4423bd29bb23f89d88e094e2956f.md)

    Copies texture data region from one buffer to one texture. Texture data in the buffer is interpreted in row-major arrangement. 

* [virtual void copy_texture_to_buffer(IBuffer *dst, u64 dst_offset, u32 dst_row_pitch, u32 dst_slice_pitch, ITexture *src, SubresourceIndex src_subresource, u32 src_x, u32 src_y, u32 src_z, u32 copy_width, u32 copy_height, u32 copy_depth)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a8d530ad1e4c1e64ef49cfc6fa46b4b98.md)

    Copies texture data region from one texture to one buffer. Texture data is written to the buffer in row-major arrangement. 

* [virtual void end_copy_pass()=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a715afb224260669bf65650b2afb9d967.md)

    Ends a copy pass. 

* [virtual void resource_barrier(Span< const BufferBarrier > buffer_barriers, Span< const TextureBarrier > texture_barriers)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a0b773d201ee15f29ed095df3da0cfcdc.md)

    Issues one resource barrier that synchronizes GPU pipeline access to multiple resources. 

* [virtual RV submit(Span< IFence * > wait_fences, Span< IFence * > signal_fences, bool allow_host_waiting)=0](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ad5abcba3617f9551e1f3e4e3e61c3f6f.md)

    Submits the recorded commands in this command buffer to the attached command queue. 

