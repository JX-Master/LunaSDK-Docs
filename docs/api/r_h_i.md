# RHI
Render Hardware [Interface](struct_luna_1_1_interface.md) (RHI) module provides uniform API to use platform's graphcis hardware (GPU) to accelerate rendering and parallel computing tasks. 

## Topics
* [RHI Errors](r_h_i_error.md)
## Types
* [Luna::RHI::IAdapter](struct_luna_1_1_r_h_i_1_1_i_adapter.md)

    Represents a physical graphics device installed on the platform. 


* [Luna::RHI::BufferDesc](struct_luna_1_1_r_h_i_1_1_buffer_desc.md)

    Describes one [IBuffer](struct_luna_1_1_r_h_i_1_1_i_buffer.md) object. 


* [Luna::RHI::IBuffer](struct_luna_1_1_r_h_i_1_1_i_buffer.md)

    Represents one buffer resource that can be used to contain arbitrary binary data. 


* [Luna::RHI::TextureBarrier](struct_luna_1_1_r_h_i_1_1_texture_barrier.md)

    Describes one texture barrier. 


* [Luna::RHI::BufferBarrier](struct_luna_1_1_r_h_i_1_1_buffer_barrier.md)

    Describes one buffer barrier. 


* [Luna::RHI::Viewport](struct_luna_1_1_r_h_i_1_1_viewport.md)

    Describes one viewport used by [ICommandBuffer::set_viewport](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1ade5bc1a0f452cc3e355040ae00499efb.md) and [ICommandBuffer::set_viewports](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1abe3f9b469aa3574cd81974f7523f9cac.md). 


* [Luna::RHI::ColorAttachment](struct_luna_1_1_r_h_i_1_1_color_attachment.md)

    Describes one color attachment when beginning a render pass. 


* [Luna::RHI::DepthStencilAttachment](struct_luna_1_1_r_h_i_1_1_depth_stencil_attachment.md)

    Describes one depth stencil attachment when beginning a render pass. 


* [Luna::RHI::ResolveAttachment](struct_luna_1_1_r_h_i_1_1_resolve_attachment.md)

    Describes one resolve attachment when beginning a render pass. 


* [Luna::RHI::RenderPassDesc](struct_luna_1_1_r_h_i_1_1_render_pass_desc.md)

    Describes one render pass. 


* [Luna::RHI::ComputePassDesc](struct_luna_1_1_r_h_i_1_1_compute_pass_desc.md)

    Describes one compute pass. 


* [Luna::RHI::CopyPassDesc](struct_luna_1_1_r_h_i_1_1_copy_pass_desc.md)

    Describes one copy pass. 


* [Luna::RHI::VertexBufferView](struct_luna_1_1_r_h_i_1_1_vertex_buffer_view.md)

    Describes one vertex buffer view when binding one vertex buffer to the render pipeline. 


* [Luna::RHI::IndexBufferView](struct_luna_1_1_r_h_i_1_1_index_buffer_view.md)

    Describes one index buffer view when binding one index buffer to the render pipeline. 


* [Luna::RHI::ICommandBuffer](struct_luna_1_1_r_h_i_1_1_i_command_buffer.md)

    Used to allocate memory for commands, record commands, submitting commands to GPU and tracks the state of the submitted commands. 


* [Luna::RHI::BufferViewDesc](struct_luna_1_1_r_h_i_1_1_buffer_view_desc.md)

    Describes one buffer view in descriptor set. 


* [Luna::RHI::TextureViewDesc](struct_luna_1_1_r_h_i_1_1_texture_view_desc.md)

    Describes one texture view in descriptor set. 


* [Luna::RHI::SamplerDesc](struct_luna_1_1_r_h_i_1_1_sampler_desc.md)

    Describes one sampler in descriptor set. 


* [Luna::RHI::DescriptorSetDesc](struct_luna_1_1_r_h_i_1_1_descriptor_set_desc.md)

    Describes one descriptor set. 


* [Luna::RHI::WriteDescriptorSet](struct_luna_1_1_r_h_i_1_1_write_descriptor_set.md)

    Describes one descriptor set write operation. Every descriptor set write operation may update one continuous range of descriptors in the same binding slot. 


* [Luna::RHI::IDescriptorSet](struct_luna_1_1_r_h_i_1_1_i_descriptor_set.md)

    Describes which views and samples are bound to the pipeline. This can be set at any time before the draw call or dispatch call is submitted. 


* [Luna::RHI::DescriptorSetLayoutBinding](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_binding.md)

    Describes one binding in one descriptor set. 


* [Luna::RHI::DescriptorSetLayoutDesc](struct_luna_1_1_r_h_i_1_1_descriptor_set_layout_desc.md)

    Specifies one descriptor set layout. 


* [Luna::RHI::IDescriptorSetLayout](struct_luna_1_1_r_h_i_1_1_i_descriptor_set_layout.md)

    Represents one descriptor set layout that can be used to create descriptor sets and pipeline layouts. 


* [Luna::RHI::DeviceFeatureData](struct_luna_1_1_r_h_i_1_1_device_feature_data.md)

    Represents the device feature check result. 


* [Luna::RHI::CommandQueueDesc](struct_luna_1_1_r_h_i_1_1_command_queue_desc.md)

    Describes one command queue. 


* [Luna::RHI::IDevice](struct_luna_1_1_r_h_i_1_1_i_device.md)

    Represents one logical graphic device on the platform. 


* [Luna::RHI::IDeviceChild](struct_luna_1_1_r_h_i_1_1_i_device_child.md)

    Represents one object that is created by [IDevice](struct_luna_1_1_r_h_i_1_1_i_device.md) and is only available in the device context. 


* [Luna::RHI::IDeviceMemory](struct_luna_1_1_r_h_i_1_1_i_device_memory.md)

    Represents one allocated device memory. 


* [Luna::RHI::IFence](struct_luna_1_1_r_h_i_1_1_i_fence.md)

    Represents a synchronization object that can be used to synchronize commands executed in different command queues. 


* [Luna::RHI::PipelineLayoutDesc](struct_luna_1_1_r_h_i_1_1_pipeline_layout_desc.md)

    Describes one pipeline layout. 


* [Luna::RHI::IPipelineLayout](struct_luna_1_1_r_h_i_1_1_i_pipeline_layout.md)

    Describes how shader parameters are accessed by every shader in the pipeline. 


* [Luna::RHI::ShaderData](struct_luna_1_1_r_h_i_1_1_shader_data.md)

    Specify one shader data. 


* [Luna::RHI::ComputePipelineStateDesc](struct_luna_1_1_r_h_i_1_1_compute_pipeline_state_desc.md)

    Describes pipeline configurations of one compute pipeline. 


* [Luna::RHI::InputAttributeDesc](struct_luna_1_1_r_h_i_1_1_input_attribute_desc.md)

    Describes one attribute in the input layout. 


* [Luna::RHI::InputBindingDesc](struct_luna_1_1_r_h_i_1_1_input_binding_desc.md)

    Describes one input buffer binding. 


* [Luna::RHI::InputLayoutDesc](struct_luna_1_1_r_h_i_1_1_input_layout_desc.md)

    Describes the vertex input layout for the graphics pipeline. 


* [Luna::RHI::AttachmentBlendDesc](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc.md)

    Describes the blending configurations for one attachment. 


* [Luna::RHI::BlendDesc](struct_luna_1_1_r_h_i_1_1_blend_desc.md)

    Describes blending configurations for one graphics pipeline. 


* [Luna::RHI::RasterizerDesc](struct_luna_1_1_r_h_i_1_1_rasterizer_desc.md)

    Describes rasterizer configurations for one graphics pipeline. 


* [Luna::RHI::DepthStencilOpDesc](struct_luna_1_1_r_h_i_1_1_depth_stencil_op_desc.md)

    Describes the depth stencil operation. 


* [Luna::RHI::DepthStencilDesc](struct_luna_1_1_r_h_i_1_1_depth_stencil_desc.md)

    Describes depth stencil stage configurations of one graphics pipeline. 


* [Luna::RHI::GraphicsPipelineStateDesc](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc.md)

    Describes pipeline configurations of one compute pipeline. 


* [Luna::RHI::IPipelineState](struct_luna_1_1_r_h_i_1_1_i_pipeline_state.md)

    Represents one pipeline state object that stores pipeline configurations that can be applied to one pipeline in one call. 


* [Luna::RHI::PipelineStatistics](struct_luna_1_1_r_h_i_1_1_pipeline_statistics.md)

    Specifies one query in pipeline statistics query heap. 


* [Luna::RHI::QueryHeapDesc](struct_luna_1_1_r_h_i_1_1_query_heap_desc.md)

    Describes one query heap. 


* [Luna::RHI::IQueryHeap](struct_luna_1_1_r_h_i_1_1_i_query_heap.md)

    Contains one array of query elements that can be used to query pipeline execution information, such as pixel occlusion, execution time and pipeline statistics. 


* [Luna::RHI::SubresourceIndex](struct_luna_1_1_r_h_i_1_1_subresource_index.md)

    Specifies the index pair of one subresource in one texture resource. 


* [Luna::RHI::IResource](struct_luna_1_1_r_h_i_1_1_i_resource.md)

    Represents a memory region that can be accessed by GPU. 


* [Luna::RHI::SwapChainDesc](struct_luna_1_1_r_h_i_1_1_swap_chain_desc.md)

    Describes one swap chain. 


* [Luna::RHI::ISwapChain](struct_luna_1_1_r_h_i_1_1_i_swap_chain.md)

    Represents one swap chain used for presenting images to the screen. 


* [Luna::RHI::TextureDesc](struct_luna_1_1_r_h_i_1_1_texture_desc.md)

    Describes one texture resource. 


* [Luna::RHI::DepthStencilValue](struct_luna_1_1_r_h_i_1_1_depth_stencil_value.md)

    Describes one pair of depth and stencil values used for clearing depth stencil attachments. 


* [Luna::RHI::ClearValue](struct_luna_1_1_r_h_i_1_1_clear_value.md)

    Describes one clear value used to specify optimized clear value for texture resources. 


* [Luna::RHI::ITexture](struct_luna_1_1_r_h_i_1_1_i_texture.md)

    Represents one texture resource that can be used to contain pixel data of certain format. 


* [Luna::RHI::CopyResourceData](struct_luna_1_1_r_h_i_1_1_copy_resource_data.md)

    Specifies one resource data copy operation. 


## Enumerations
* [Luna::RHI::BufferUsageFlag](group___r_h_i_1ga22283687fb8acafd6ad0ddb5b8e71920.md)

    Specifies possible usages for one [IBuffer](struct_luna_1_1_r_h_i_1_1_i_buffer.md) object. 

* [Luna::RHI::ResourceBarrierFlag](group___r_h_i_1ga1291495222dfa5429c7578cec7a0bf99.md)

    Specifies additional flags for one buffer or texture barrier. 

* [Luna::RHI::BufferStateFlag](group___r_h_i_1ga44197ca8c7fae3c510e42a6c9b5536bd.md)

    Specifies buffer resource states before and after one barrier. 

* [Luna::RHI::TextureStateFlag](group___r_h_i_1gabfe469f739b00632e7855e0b9e775fe6.md)

    Specifies texture resource states before and after one barrier. 

* [Luna::RHI::LoadOp](group___r_h_i_1ga8d353cef0bd83ad8a6b73532498b26ee.md)

    The operation to perform when the attachment is loaded to GPU. 

* [Luna::RHI::StoreOp](group___r_h_i_1ga25180578f42b085cc80df254689bd318.md)

    The operation to perform when the render texture is written back to resource memory. 

* [Luna::RHI::OcclusionQueryMode](group___r_h_i_1gadb853a4372dbf06383840034406e0cb9.md)

    Specifies the occlusion query working mode. 

* [Luna::RHI::Filter](group___r_h_i_1gaa7b87805d61bd375f6345014a3d028c8.md)

    Specifies the filtering mode for samplers. 

* [Luna::RHI::TextureAddressMode](group___r_h_i_1gaf6eef5ace6d21fcf0d846e6950ed179d.md)

    Specifies the texture address mode for samplers when the sample position does not fall in range [0, 1]. 

* [Luna::RHI::BorderColor](group___r_h_i_1ga1a662a7828db25444a79202c99a11b34.md)

    Specifies the border color to use if texture address mode is [TextureAddressMode::border](group___r_h_i_1ggaf6eef5ace6d21fcf0d846e6950ed179da2de42fbb00305f8282310f1b3e10ce9a.md). 

* [Luna::RHI::DescriptorType](group___r_h_i_1ga44b9ba38881a2ddef7849d710aa216e2.md)

    Specifies the type of descriptors that can be placed in a descriptor set. 

* [Luna::RHI::TextureViewType](group___r_h_i_1ga4e4acbc44dbd67b766e76abada8c0ff9.md)

    Specifies the texture view type, which is how render pipeline interprets texture data. 

* [Luna::RHI::ShaderVisibilityFlag](group___r_h_i_1ga4dfc1279e665f25cb66d7bcfacfb796f.md)

    Specifies which shader can access descriptors in the specified binding. 

* [Luna::RHI::DescriptorSetLayoutFlag](group___r_h_i_1ga999e242f3410baeb0f177d9b21e0eead.md)

    Specifies additional flags for one descriptor set layout. 

* [Luna::RHI::DeviceFeature](group___r_h_i_1ga4200fb69a6165d0624a052e798e58181.md)

    Specifies device features that can be queried at run time. 

* [Luna::RHI::CommandQueueType](group___r_h_i_1gaa56792d4f26b9c3a4d314cd3a662ae73.md)

    Specifies command queue types. 

* [Luna::RHI::CommandQueueFlag](group___r_h_i_1gaaa41659a673405f1b0553989ed7bc8ed.md)

    Specifies additional flags for command queues. 

* [Luna::RHI::MemoryType](group___r_h_i_1gaebe724447eeccdbd8ea4fad8b0a49c2d.md)

    Specify the memory type. See remarks for details. 

* [Luna::RHI::PipelineLayoutFlag](group___r_h_i_1ga76f65c5515fa3b6850d6d2a3a45f7622.md)

    Describes attributes of one pipeline layout object. 

* [Luna::RHI::ShaderDataFormat](group___r_h_i_1ga41181cc4822b7c0041d7a0f3764bd09c.md)

    Specify shader data format. 

* [Luna::RHI::InputRate](group___r_h_i_1gad940447931d955a6a7f7817a04713e9a.md)

    The input rate for one input attribute (per vertex or per instance). 

* [Luna::RHI::BlendFactor](group___r_h_i_1gaff6a69260c6a522886b802c33f58601e.md)

    Specifies the blend factor used for blending. 

* [Luna::RHI::BlendOp](group___r_h_i_1gab79444a2c036a01a98a1472131439694.md)

    Specifies the blend operation. 

* [Luna::RHI::ColorWriteMask](group___r_h_i_1ga239d4ff9cc6e1ece57aeafb9d1d5b1bc.md)

    Identifies which components of each pixel of a attachment are writable during blending. 

* [Luna::RHI::FillMode](group___r_h_i_1gac81ec815b912a0d19626f2f8f9fc1f7f.md)

    Describes triangle fill mode of the rasterizer. 

* [Luna::RHI::CullMode](group___r_h_i_1ga83a4de96ca6b10185b522a00265f0287.md)

    Describes cull mode of the rasterizer. 

* [Luna::RHI::StencilOp](group___r_h_i_1ga32d851e8611e5ee5cc3af7419204e23f.md)

    Specifies the stencil operation to perform when stencil test passed or failed. 

* [Luna::RHI::CompareFunction](group___r_h_i_1ga2b89d3ba24bde15c71c7c433be96c8a4.md)

    Specifies the compare function used for comparison. 

* [Luna::RHI::IndexBufferStripCutValue](group___r_h_i_1ga63497036099cee50e2a03d13bbda77f1.md)

    The value used to finish an existing line or triangle strip and start a new one when [GraphicsPipelineStateDesc::primitive_topology](struct_luna_1_1_r_h_i_1_1_graphics_pipeline_state_desc_1ad17233c42429f8e9367f7b3b29e2e98a.md) is set to [PrimitiveTopology::line_strip](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333fa7441cbdc45313ce65d3606b1d6e403dd.md) or [PrimitiveTopology::triangle_strip](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333fa01edf5f1ae6135daec55d230c83d3885.md). 

* [Luna::RHI::PrimitiveTopology](group___r_h_i_1ga04e2e034a02712bbeb2937de1f8c333f.md)

    Specifies the primitive type for the graphics pipeline to draw. 

* [Luna::RHI::QueryType](group___r_h_i_1ga3535755f4ab3d7d84c876227034d826b.md)

    Specifies query type. 

* [Luna::RHI::ResourceFlag](group___r_h_i_1gafecaf207868d67e85baf5514b3c9bdd6.md)

    Specifies additional flags for one resource. 

* [Luna::RHI::BackendType](group___r_h_i_1ga4da0d14d49c5f620d126d5cc3fdc2a33.md)

    Lists supported RHI backends (implementation APIs). 

* [Luna::RHI::Format](group___r_h_i_1ga702d9f1f694087ebf8f85708f2825914.md)

    Describes data formats for vertices and pixels in RHI. 

* [Luna::RHI::TextureType](group___r_h_i_1ga3ed048732590d47e986a407d4be55746.md)

    Specifies the texture type. 

* [Luna::RHI::TextureUsageFlag](group___r_h_i_1ga158288d119b258c9a2dc7c2ca0cd2501.md)

    Specifies possible usages of one texture resource. 

* [Luna::RHI::ClearValueType](group___r_h_i_1ga4697a0b057914028860d7c84f04a0d76.md)

    Specifies the clear value type used. 

* [Luna::RHI::ResourceDataCopyOp](group___r_h_i_1gae43d83f61c5bb37ebf85b04d5f007353.md)

    Specifies the type of one resource data copy operation. 

## Constants
* [constexpr SubresourceIndex TEXTURE_BARRIER_ALL_SUBRESOURCES](group___r_h_i_1gae1ebf3b256a5d406c1fd4ef77f508572.md)

    A special number that selects all subresources of one resource for one barrier operation. 

* [constexpr u32 DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md)

    A special number that identifies the query operation is disabled. 

## Functions
* [Vector< Ref< IAdapter > > get_adapters()](group___r_h_i_1ga9b43c46b4732a021d76e3783ac4f7ac4.md)

    Gets a list of adapters installed on the platform. 

* [R< Ref< IDevice > > new_device(IAdapter *adapter)](group___r_h_i_1gafba37e8bce43bb5aeb71faafcff4ffcc.md)

    Creates one device using the specified adapter. 

* [IDevice * get_main_device()](group___r_h_i_1ga83ddbe24ec26ca8ffd52552b35939424.md)

    Gets the main device of the platform. 

* [BackendType get_backend_type()](group___r_h_i_1ga3092e6eafa049de1dd2915b32dfa715b.md)

    Gets the backend type. 

* [ShaderCompiler::TargetFormat get_current_platform_shader_target_format()](group___r_h_i_1gac1f9af9ae978dd9345fbaec3416d7f43.md)

    Gets the desired shader compile target format that can be used for the current graphics API. 

* [ShaderData get_shader_data_from_compile_result(const ShaderCompiler::ShaderCompileResult &compile_result)](group___r_h_i_1ga6cc479bc5472863690913fb196104fc7.md)

    Gets one [ShaderData](struct_luna_1_1_r_h_i_1_1_shader_data.md) structure that referrs the specified compile result. 

* [void fill_compute_pipeline_state_desc_from_compile_result(ComputePipelineStateDesc &desc, const ShaderCompiler::ShaderCompileResult &compile_result)](group___r_h_i_1ga3bdfcaf78133a47b0d13740916901d90.md)

    Fills `cs`, `metal_numthreads_x`, `metal_numthreads_y` and `metal_numthreads_z` properties of [ComputePipelineStateDesc](struct_luna_1_1_r_h_i_1_1_compute_pipeline_state_desc.md) using shader compile results. 

* [usize bits_per_pixel(Format format)](group___r_h_i_1ga8f6963a1072a1eda3f8e68ae53aec30f.md)

    Gets the size of one pixel in the specified format, in bits. 

* [RV copy_resource_data(ICommandBuffer *command_buffer, Span< const CopyResourceData > copies)](group___r_h_i_1ga449298504cd2e477f2b5534d05290896.md)

    Copies data between host memory and resource memory. 

