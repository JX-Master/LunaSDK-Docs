# Luna::RG::IRenderGraph::get_render_pass

```c++
virtual IRenderPass * get_render_pass(usize index)=0
```

Gets the render pass object of the specified render pass. 



## Parameters
* *in* **index**

    The index of the render pass to get. 

## Return value
Returns the render pass object of the specified render pass. Returns `nullptr` if the index is not valid, or [compile](struct_luna_1_1_r_g_1_1_i_render_graph_1a5e1798a7bcfbadcc7e45b88c23736b10.md) is not called. 

