# Luna::RG::IRenderGraph::get_enabled_render_passes

```c++
virtual void get_enabled_render_passes(Vector< usize > &render_passes)=0
```

Gets all enabled render passes. 

This should be called after [compile](struct_luna_1_1_r_g_1_1_i_render_graph_1a5e1798a7bcfbadcc7e45b88c23736b10.md), or no render pass will be returned. 

## Parameters
* *out* **render_passes**

    Returns the array of indices of enabled render passes. 

