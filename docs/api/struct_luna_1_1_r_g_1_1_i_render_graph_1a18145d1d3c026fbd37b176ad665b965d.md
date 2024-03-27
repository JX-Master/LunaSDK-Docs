# Luna::RG::IRenderGraph::set_desc

```c++
virtual void set_desc(const RenderGraphDesc &desc)=0
```

Sets the descriptor of this render graph. 

The user should call [compile](struct_luna_1_1_r_g_1_1_i_render_graph_1a5e1798a7bcfbadcc7e45b88c23736b10.md) after setting the descriptor in order to make the new descriptor take effect. 

## Parameters
* *in* **desc**

    The descriptor to set. 

