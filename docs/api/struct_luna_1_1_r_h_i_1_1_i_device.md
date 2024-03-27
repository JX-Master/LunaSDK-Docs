# Luna::RHI::IDevice
Represents one logical graphic device on the platform. 

```c++
interface Luna::RHI::IDevice : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual DeviceFeatureData check_feature(DeviceFeature feature)=0](struct_luna_1_1_r_h_i_1_1_i_device_1ab07056e86da3287e2c411ff00055bedb.md)

    Checks device feature. 

* [virtual void get_texture_data_placement_info(u32 width, u32 height, u32 depth, Format format, u64 *size=nullptr, u64 *alignment=nullptr, u64 *row_pitch=nullptr, u64 *slice_pitch=nullptr)=0](struct_luna_1_1_r_h_i_1_1_i_device_1ad6ee8198289369f6401069251875ef1c.md)

    Gets the texture data placement information when storing texture data in a buffer. The texture data is arranged in row-major order. 

* [virtual R< Ref< IBuffer > > new_buffer(MemoryType memory_type, const BufferDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a23b0fa86e9cab7ad3633e1ff821e2477.md)

    Creates one new buffer resource and allocates device memory for the resource. 

* [virtual R< Ref< ITexture > > new_texture(MemoryType memory_type, const TextureDesc &desc, const ClearValue *optimized_clear_value=nullptr)=0](struct_luna_1_1_r_h_i_1_1_i_device_1af2ef0567a0af594338f92b2c5a73e552.md)

    Creates one new texture resource and allocates device memory for the resource. 

* [virtual bool is_resources_aliasing_compatible(MemoryType memory_type, Span< const BufferDesc > buffers, Span< const TextureDesc > textures)=0](struct_luna_1_1_r_h_i_1_1_i_device_1ad14346f9d7c54786c278dab256d19866.md)

    Checks whether the given resources can share the same device memory. 

* [virtual R< Ref< IDeviceMemory > > allocate_memory(MemoryType memory_type, Span< const BufferDesc > buffers, Span< const TextureDesc > textures)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a7f66da6302fcb28668f8322a0a122941.md)

    Allocates device memory that is capable of storing resources specified. 

* [virtual R< Ref< IBuffer > > new_aliasing_buffer(IDeviceMemory *device_memory, const BufferDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a869511b830ca47ff0cd34e4013f192f2.md)

    Creates one aliasing buffer that shares the same device memory with the existing resource. 

* [virtual R< Ref< ITexture > > new_aliasing_texture(IDeviceMemory *device_memory, const TextureDesc &desc, const ClearValue *optimized_clear_value=nullptr)=0](struct_luna_1_1_r_h_i_1_1_i_device_1ab37f5ea34435d671a12463c095a3029a.md)

    Creates one aliasing texture that shares the same device memory with the existing resource. 

* [virtual R< Ref< IPipelineLayout > > new_pipeline_layout(const PipelineLayoutDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a558196bb48270ecf2b0d17ddadc6c026.md)

    Creates one new pipeline layout. 

* [virtual R< Ref< IPipelineState > > new_graphics_pipeline_state(const GraphicsPipelineStateDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a35080f6d09438c480307b04047c2dc30.md)

    Creates one new graphic pipeline state. 

* [virtual R< Ref< IPipelineState > > new_compute_pipeline_state(const ComputePipelineStateDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1af4949fd443367a6538a4b755bdfad245.md)

    Creates one compute pipeline state. 

* [virtual R< Ref< IDescriptorSetLayout > > new_descriptor_set_layout(const DescriptorSetLayoutDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1aaec32b029d328785332fe8b5282a7cba.md)

    Creates one new descriptor set layout object that can be used to create descriptor sets. 

* [virtual R< Ref< IDescriptorSet > > new_descriptor_set(const DescriptorSetDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a4f230666aa612d0b572ad1588e0f1c28.md)

    Creates one new descriptor set object that describes resources that are bound to the pipeline. 

* [virtual u32 get_num_command_queues()=0](struct_luna_1_1_r_h_i_1_1_i_device_1a014bf6e47efb7cc415dd71c68912b296.md)

    Gets the number of command queues of the device. 

* [virtual CommandQueueDesc get_command_queue_desc(u32 command_queue_index)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a683366c558eb77526a21ba4ec52e6e1d.md)

    Gets the command queue descriptor of the specified command queue. 

* [virtual R< Ref< ICommandBuffer > > new_command_buffer(u32 command_queue_index)=0](struct_luna_1_1_r_h_i_1_1_i_device_1abe939b9ef330ef94120c1dc1cb96c806.md)

    Creates one command buffer. 

* [virtual R< f64 > get_command_queue_timestamp_frequency(u32 command_queue_index)=0](struct_luna_1_1_r_h_i_1_1_i_device_1ac868409c6ccfb1010f64373db0f0235d.md)

    Gets the GPU timestamp frequency of the specified command queue. The timestamp frequency is measured in ticks per second. 

* [virtual R< Ref< IQueryHeap > > new_query_heap(const QueryHeapDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a176f79372425381749474bc3587b473f.md)

    Creates one new query heap that can be used to store GPU query result. 

* [virtual R< Ref< IFence > > new_fence()=0](struct_luna_1_1_r_h_i_1_1_i_device_1a2827029139a65d855b00c995d898abb7.md)

    Creates one new fence that can be used to synchronize execution of multiple command buffers. 

* [virtual R< Ref< ISwapChain > > new_swap_chain(u32 command_queue_index, Window::IWindow *window, const SwapChainDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_device_1a0e5654d426db531b47a4dbcae73b044c.md)

    Creates one swap chain and binds it to the specified window. 

