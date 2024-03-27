# Luna::RG::RenderGraphConnection
Describes one input or output connection between the resource node and the render pass node in one render graph. 

```c++
struct Luna::RG::RenderGraphConnection
```

## Member objects
* [usize pass](struct_luna_1_1_r_g_1_1_render_graph_connection_1afc87f2078fc5631a6c3a920ab345642e.md)

    The index of the connected render pass node in [RenderGraphDesc::passes](struct_luna_1_1_r_g_1_1_render_graph_desc_1a133bc7b9c234c96238d19033841d2fe5.md). 

* [Name parameter](struct_luna_1_1_r_g_1_1_render_graph_connection_1a445f7fb73ded52dd9cc5295180edebeb.md)

    The name of the render pass parameter to bind the resource to. 

* [usize resource](struct_luna_1_1_r_g_1_1_render_graph_connection_1af0d839dc5dac29e2c36bc6843316b1f1.md)

    The index of the connected resource node in [RenderGraphDesc::resources](struct_luna_1_1_r_g_1_1_render_graph_desc_1a0f01a4557f52bfb35df5037f9d73f2a0.md). 

