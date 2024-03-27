# Luna::RG::RenderGraphDesc
Describes one render graph. 

```c++
struct Luna::RG::RenderGraphDesc
```

## Member objects
* [Vector<RenderGraphPassNode> passes](struct_luna_1_1_r_g_1_1_render_graph_desc_1a133bc7b9c234c96238d19033841d2fe5.md)

    The array of passed in this render graph. The order of elements this array will be the execution order of render passes. 

* [Vector<RenderGraphResourceNode> resources](struct_luna_1_1_r_g_1_1_render_graph_desc_1a0f01a4557f52bfb35df5037f9d73f2a0.md)

    The array of resources in this render graph. 

* [Vector<RenderGraphConnection> input_connections](struct_luna_1_1_r_g_1_1_render_graph_desc_1aaee4d83b2c61fdcfee45c932c1c5e2e3.md)

    The array of input connections (resource -> pass). 

* [Vector<RenderGraphConnection> output_connections](struct_luna_1_1_r_g_1_1_render_graph_desc_1af42768c5a209e6d230dd5f05fa33d60c.md)

    The array of output connection (pass -> resource). 

