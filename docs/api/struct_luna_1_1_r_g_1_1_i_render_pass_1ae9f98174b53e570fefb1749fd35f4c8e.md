# Luna::RG::IRenderPass::execute

```c++
virtual RV execute(IRenderPassContext *ctx)=0
```

Executes the render pass. This is called by the render graph in [IRenderGraph::execute](struct_luna_1_1_r_g_1_1_i_render_graph_1a3d0d87f0163abaa978da54d1ba45610c.md), the user should not call this manually. 



## Parameters
* *in* **ctx**

    The render graph execution context that can be used by the render pass to read input / output resources, get command buffers, allocate temporary resources and so on. 

