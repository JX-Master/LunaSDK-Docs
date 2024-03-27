# Luna::RG::IRenderGraph
Represents one render graph that can be used to schedule render passes and reuse in-frame transient render resources to reduce memory comsumption. 

```c++
interface Luna::RG::IRenderGraph : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual RHI::IDevice * get_device()=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a9e9c2057836469b40bd731f1040cfe32.md)

    Gets the RHI device attached to this render graph. 

* [virtual const RenderGraphDesc & get_desc()=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a464647156e5442038d13151bd44d4840.md)

    Gets the descriptor of this render graph. 

* [virtual void set_desc(const RenderGraphDesc &desc)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a18145d1d3c026fbd37b176ad665b965d.md)

    Sets the descriptor of this render graph. 

* [virtual RV compile(const RenderGraphCompileConfig &config)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a5e1798a7bcfbadcc7e45b88c23736b10.md)

    Compiles the render graph. 

* [virtual void get_enabled_render_passes(Vector< usize > &render_passes)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1ade3e5438b0a2dc5f563042a799a96b55.md)

    Gets all enabled render passes. 

* [virtual IRenderPass * get_render_pass(usize index)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a096321ae30d99afaeacb1048868c009c.md)

    Gets the render pass object of the specified render pass. 

* [virtual void set_external_resource(usize index, RHI::IResource *resource)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1aac88548caf5a3e8889fb8dc3fad0bc6d.md)

    Sets external resource. 

* [virtual RV execute(RHI::ICommandBuffer *cmdbuf)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a3d0d87f0163abaa978da54d1ba45610c.md)

    Executes the render graph. 

* [virtual RHI::IResource * get_persistent_resource(usize index)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a55900c765cba6a4c711754f2991315ce.md)

    Gets one persistent resource. 

* [virtual RV get_pass_time_intervals(Vector< u64 > &pass_times)=0](struct_luna_1_1_r_g_1_1_i_render_graph_1a67280696e8651b416319b524c091bebd.md)

    Gets the time used for every active render pass. 

