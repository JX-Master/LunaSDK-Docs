# Luna::RG::IRenderPassContext::release_temporary_resource

```c++
virtual void release_temporary_resource(RHI::IResource *res)=0
```

Releases the temporary resource allocated from [allocate_temporary_resource](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a6cff7ae113c19abb66cc6219c4ed0bc6.md). 

This call will make the resource immediately reusable for other temporary resource allocation calls, so that another call to [allocate_temporary_resource](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a6cff7ae113c19abb66cc6219c4ed0bc6.md) in the same render pass may reuse the released resource, thus reduces memory comsumption. If the resource is not released by this call, it will be released at the end of the render pass. 

## Parameters
* *in* **res**

    The resource to release. 

