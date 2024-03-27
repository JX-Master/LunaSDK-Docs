# Luna::RHI::AttachmentBlendDesc
Describes the blending configurations for one attachment. 

```c++
struct Luna::RHI::AttachmentBlendDesc
```

## Member objects
* [bool blend_enable](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1a9e21a3c944b093d8f005f5c6c298a7a4.md)

    Whether to enable color blending for this attachment. If this is `false`, pixels outputted by the graphics pipeline will overwrite existing pixels directly if they are not discarded in pixel shader. 

* [BlendFactor src_blend_color](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1aedd3f41a6f43c4368a32b0ec68668bbc.md)

    The blend factor used for the source color. 

* [BlendFactor dst_blend_color](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1a4e6f8954896fe9b9ae911b79980de7bd.md)

    The blend factor used for the destination color. 

* [BlendOp blend_op_color](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1a0b2d0035a5ac966dc822b4bdc405dbaf.md)

    The blend operation used for color blending. 

* [BlendFactor src_blend_alpha](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1afce6d421d64113b0d505f90477174379.md)

    The blend factor used for the source alpha. 

* [BlendFactor dst_blend_alpha](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1a7658dfe2c457273bc59a8f9172b58b62.md)

    The blend factor used for the destination alpha. 

* [BlendOp blend_op_alpha](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1af6636e554cdd69cec45ecd7cce3f3367.md)

    The blend operation used for alpha blending. 

* [ColorWriteMask color_write_mask](struct_luna_1_1_r_h_i_1_1_attachment_blend_desc_1aeabad54acfed269382d59493fffef37e.md)

    The color components that can be modified during blending. 

