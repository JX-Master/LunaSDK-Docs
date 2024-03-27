# Luna::RHI::ClearValue
Describes one clear value used to specify optimized clear value for texture resources. 

```c++
struct Luna::RHI::ClearValue
```

## Member objects
* [Format format](struct_luna_1_1_r_h_i_1_1_clear_value_1a751c4987b2c6908c70a915ab18d36653.md)

    The format of the texture. 

* [ClearValueType type](struct_luna_1_1_r_h_i_1_1_clear_value_1a4c201b9d911922b933aae1ca8ca6cabc.md)

    The type of the clear value. 

* [f32 color[4]](struct_luna_1_1_r_h_i_1_1_clear_value_1affad11157b63d4d2107c386cc8e645b0.md)

    The clear color to use if `type` is ClearValueType::color. 

* [DepthStencilValue depth_stencil](struct_luna_1_1_r_h_i_1_1_clear_value_1ac6118bde2829ede2b6cf3e91ac2e5a02.md)

    The depth stencil clear value to use if `type` is ClearValueType::depth_stencil. 

