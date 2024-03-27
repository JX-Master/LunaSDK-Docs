# Luna::RHI::ICommandBuffer::set_blend_factor

```c++
virtual void set_blend_factor(const Float4U &blend_factor)=0
```

Sets the blend factor of the graphics pipeline. 

The blend factor is used if [BlendFactor::blend_factor](group___r_h_i_1ggaff6a69260c6a522886b802c33f58601ea9f34717047b7e045aba4fdf173e020c2.md) or [BlendFactor::one_minus_blend_factor](group___r_h_i_1ggaff6a69260c6a522886b802c33f58601eab7df0c0346b8921262b22a7d8ca1a902.md) is used for any blending operation in [BlendDesc](struct_luna_1_1_r_h_i_1_1_blend_desc.md) of the binding graphics pipeline state object. 

## Parameters
* *in* **blend_factor**

    The blend factor (in RGBA order) to set. 

