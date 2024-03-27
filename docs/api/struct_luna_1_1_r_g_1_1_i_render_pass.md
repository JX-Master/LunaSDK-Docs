# Luna::RG::IRenderPass
Represents one user-implemented render pass. 

```c++
interface Luna::RG::IRenderPass : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual RV execute(IRenderPassContext *ctx)=0](struct_luna_1_1_r_g_1_1_i_render_pass_1ae9f98174b53e570fefb1749fd35f4c8e.md)

    Executes the render pass. This is called by the render graph in [IRenderGraph::execute](struct_luna_1_1_r_g_1_1_i_render_graph_1a3d0d87f0163abaa978da54d1ba45610c.md), the user should not call this manually. 

