# Luna::RHI::BlendDesc
Describes blending configurations for one graphics pipeline. 

```c++
struct Luna::RHI::BlendDesc
```

## Member objects
* [bool alpha_to_coverage_enable](struct_luna_1_1_r_h_i_1_1_blend_desc_1a34a3e9e24fde6dc1da0ca473b9eee558.md)

    Whether to use the alpha value outputted from pixel shader as the coverage value to compute sample coverage mask in MSAA pipelines. 

* [bool independent_blend_enable](struct_luna_1_1_r_h_i_1_1_blend_desc_1a7a7608df81a902fa87e2ed43aeb7a8a6.md)

    Whether to use independent blending configurations for every attachment. 

* [AttachmentBlendDesc attachments[8]](struct_luna_1_1_r_h_i_1_1_blend_desc_1a3566beb6c1e9d185ea42b81f833153d6.md)

    The blending configurations for each attachment. 

