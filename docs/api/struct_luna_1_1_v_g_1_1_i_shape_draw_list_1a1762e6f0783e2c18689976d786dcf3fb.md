# Luna::VG::IShapeDrawList::set_texture

```c++
virtual void set_texture(RHI::ITexture *tex)=0
```

Sets the texture to be sampled when rendering the succeeding shapes. 



## Parameters
* *in* **tex**

    The texture to set. Specify `nullptr` is allowed, which behaves the same as applying one white texture with all components set to 1.0f. 

## Remark
The draw list only stores the texture and its state as-is and provides it to the renderer when the draw list is processed by the renderer. It does not do any validation to the texture and its states. It is the user and renderer's responsibility to validate the texture and its state.


The draw list has texture being set to `nullptr` after reset. 

