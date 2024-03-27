# Luna::RG::IRenderPassContext
Represents one render graph execution context. This is used only as the parameter of [IRenderPass::execute](struct_luna_1_1_r_g_1_1_i_render_pass_1ae9f98174b53e570fefb1749fd35f4c8e.md). 

```c++
interface Luna::RG::IRenderPassContext : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual RHI::ICommandBuffer * get_command_buffer()=0](struct_luna_1_1_r_g_1_1_i_render_pass_context_1ade8d956f5a5ef35f93e4b4dc10c6e4fe.md)

    Gets the command buffer used to record commands for the render pass. 

* [virtual RHI::IResource * get_input(const Name &name)=0](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a8dcd0ea356d1b020ac35172e72f88249.md)

    Gets the input resource of the render pass. 

* [virtual RHI::IResource * get_output(const Name &name)=0](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a14030e5555e257d1a4bce4ba12ab1da9.md)

    Gets the output resource of the render pass. 

* [virtual RHI::IQueryHeap * get_timestamp_query_heap(u32 *begin_index, u32 *end_index)=0](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a755e17384efba7d8bd6f9cf5909e423f.md)

    Gets the timestamp query heap used to track the running time of the render pass. 

* [virtual R< Ref< RHI::IResource > > allocate_temporary_resource(const ResourceDesc &desc)=0](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a6cff7ae113c19abb66cc6219c4ed0bc6.md)

    Allocates new temporary resource that exists only in the current pass. 

* [virtual void release_temporary_resource(RHI::IResource *res)=0](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a7b2abf307538e43e8d2ce8d2ee28bb74.md)

    Releases the temporary resource allocated from [allocate_temporary_resource](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a6cff7ae113c19abb66cc6219c4ed0bc6.md). 

