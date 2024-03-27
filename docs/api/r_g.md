# Render Graph
Render Graph (RG) module provides functions to construct render pass dependency graph to automatically reuse in-frame transient render resources to reduce memory comsumption. 

## Types
* [Luna::RG::RenderGraphPassNode](struct_luna_1_1_r_g_1_1_render_graph_pass_node.md)

    Describes one render pass node in one render graph. 


* [Luna::RG::RenderGraphResourceNode](struct_luna_1_1_r_g_1_1_render_graph_resource_node.md)

    Describes one resource node in one render graph. 


* [Luna::RG::RenderGraphConnection](struct_luna_1_1_r_g_1_1_render_graph_connection.md)

    Describes one input or output connection between the resource node and the render pass node in one render graph. 


* [Luna::RG::RenderGraphDesc](struct_luna_1_1_r_g_1_1_render_graph_desc.md)

    Describes one render graph. 


* [Luna::RG::RenderGraphCompileConfig](struct_luna_1_1_r_g_1_1_render_graph_compile_config.md)

    Describes render graph compiling configurations. 


* [Luna::RG::IRenderGraph](struct_luna_1_1_r_g_1_1_i_render_graph.md)

    Represents one render graph that can be used to schedule render passes and reuse in-frame transient render resources to reduce memory comsumption. 


* [Luna::RG::ResourceDesc](struct_luna_1_1_r_g_1_1_resource_desc.md)

    Describes one render graph resource. 


* [Luna::RG::IRenderPassContext](struct_luna_1_1_r_g_1_1_i_render_pass_context.md)

    Represents one render graph execution context. This is used only as the parameter of [IRenderPass::execute](struct_luna_1_1_r_g_1_1_i_render_pass_1ae9f98174b53e570fefb1749fd35f4c8e.md). 


* [Luna::RG::IRenderPass](struct_luna_1_1_r_g_1_1_i_render_pass.md)

    Represents one user-implemented render pass. 


* [Luna::RG::IRenderGraphCompiler](struct_luna_1_1_r_g_1_1_i_render_graph_compiler.md)

    The render graph compile context. This is used only as the parameter for [render_pass_compile_func_t](group___r_g_1ga29cde016e174eac299bb35d43ac56643.md). 


* [Luna::RG::RenderPassTypeParameter](struct_luna_1_1_r_g_1_1_render_pass_type_parameter.md)

    Describes one parameter of one render pass. 


* [Luna::RG::RenderPassTypeDesc](struct_luna_1_1_r_g_1_1_render_pass_type_desc.md)

    Describes one render pass type. 


## Enumerations
* [Luna::RG::RenderGraphResourceType](group___r_g_1gae76da9a01d229922ee38eb0efec5b857.md)

    Specifies the residency type of one resource in one render graph. 

* [Luna::RG::RenderGraphResourceFlag](group___r_g_1ga92ec1fb59849b76783c76490ab3000bf.md)

    Specifies flags of one resource in one render graph. 

* [Luna::RG::ResourceType](group___r_g_1ga3a2bffc4475e3d9654bfdd8a5dad771a.md)

    Specifies one resource type in render graph. 

## Alias types
* [using render_pass_compile_func_t =  RV(object_t userdata, IRenderGraphCompiler* compiler)](group___r_g_1ga29cde016e174eac299bb35d43ac56643.md)

    The function called by the render graph to produce the render pass object using input and output resources. 

## Constants
* [constexpr usize INVALID_RESOURCE](group___r_g_1gac4e99541691ddacbcf16df365d5dcd87.md)

    A specifal value that identifies one invalid resource name in [IRenderGraphCompiler](struct_luna_1_1_r_g_1_1_i_render_graph_compiler.md). 

## Functions
* [Ref< IRenderGraph > new_render_graph(RHI::IDevice *device)](group___r_g_1ga8c8da3f56d715d3b22f2ef0ebac3b061.md)

    Creates one new render graph. 

* [void register_render_pass_type(const RenderPassTypeDesc &desc)](group___r_g_1ga4923605fb5700d618453b44b93245ee4.md)

    Registers one new render pass type. 

* [void get_render_pass_types(Vector< Name > &out_render_pass_types)](group___r_g_1ga50a51a28127fa4fadbadb62b0f8fdc94.md)

    Gets a list of render pass types registered to the system. 

* [R< RenderPassTypeDesc > get_render_pass_type_desc(const Name &render_pass)](group___r_g_1ga79597b576b3faa27c876be77e734b810.md)

    Gets the descriptor of the specified render pass. 

