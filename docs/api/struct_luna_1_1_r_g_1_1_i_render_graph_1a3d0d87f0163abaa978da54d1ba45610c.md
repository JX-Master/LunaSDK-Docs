# Luna::RG::IRenderGraph::execute

```c++
virtual RV execute(RHI::ICommandBuffer *cmdbuf)=0
```

Executes the render graph. 

This will execute all enabled render passes in order. 

## Parameters
* *in* **cmdbuf**

    The command buffer used to record render commands of this render graph. 

## Valid Usage
* [compile](struct_luna_1_1_r_g_1_1_i_render_graph_1a5e1798a7bcfbadcc7e45b88c23736b10.md) must be called before calling this function. 

