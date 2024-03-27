# Luna::RG::IRenderGraphCompiler::set_render_pass_object

```c++
virtual void set_render_pass_object(IRenderPass *render_pass)=0
```

Sets the render pass object used for executing render commands for this render pass. 

The render pass object must be set before [render_pass_compile_func_t](group___r_g_1ga29cde016e174eac299bb35d43ac56643.md) returns, or the compilation fails. 

## Parameters
* *in* **render_pass**

    The render pass to set. The render graph will keep a strong reference to this object until the render graph is destructed or recompiled. 

