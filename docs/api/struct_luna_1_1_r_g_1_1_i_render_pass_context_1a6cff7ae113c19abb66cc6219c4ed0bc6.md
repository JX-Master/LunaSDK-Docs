# Luna::RG::IRenderPassContext::allocate_temporary_resource

```c++
virtual R< Ref< RHI::IResource > > allocate_temporary_resource(const ResourceDesc &desc)=0
```

Allocates new temporary resource that exists only in the current pass. 

The allocated The resource will be released when the pass is finished, or the user can release it manually using [release_temporary_resource](struct_luna_1_1_r_g_1_1_i_render_pass_context_1a7b2abf307538e43e8d2ce8d2ee28bb74.md). 

