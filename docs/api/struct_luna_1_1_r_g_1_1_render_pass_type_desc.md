# Luna::RG::RenderPassTypeDesc
Describes one render pass type. 

```c++
struct Luna::RG::RenderPassTypeDesc
```

## Member objects
* [Vector<RenderPassTypeParameter> input_parameters](struct_luna_1_1_r_g_1_1_render_pass_type_desc_1aa6467a26efef664cc1dc784178df9bec.md)

    The resource that is used as inputs of the node. 

* [Vector<RenderPassTypeParameter> output_parameters](struct_luna_1_1_r_g_1_1_render_pass_type_desc_1a55604054f28a8568102b82357b1f30b4.md)

    The resource that is used as outputs of the node. 

* [render_pass_compile_func_t* compile](struct_luna_1_1_r_g_1_1_render_pass_type_desc_1af4004cb1c9719d494f771b3c167f0afb.md)

    The render pass compile callback function. 

* [ObjRef userdata](struct_luna_1_1_r_g_1_1_render_pass_type_desc_1a2d82fc587187f7512fe0aa007b6dc304.md)

    The optional userdata that will be passed to the compile callback function. The system keeps a strong reference to this object until module shutdown. 

