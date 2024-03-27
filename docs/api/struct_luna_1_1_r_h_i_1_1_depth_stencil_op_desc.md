# Luna::RHI::DepthStencilOpDesc
Describes the depth stencil operation. 

```c++
struct Luna::RHI::DepthStencilOpDesc
```

## Member objects
* [StencilOp stencil_fail_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_op_desc_1a879d0a1ef151f4c5855ec1570ebc4757.md)

    The operation to perform when stencil comparison failed. 

* [StencilOp stencil_depth_fail_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_op_desc_1a8620c55b03f982f980a09c2e2f84edb0.md)

    The operation to perform when stencil comparison passed, but depth test failed. 

* [StencilOp stencil_pass_op](struct_luna_1_1_r_h_i_1_1_depth_stencil_op_desc_1a3ba7ea7c1047f3f4f816063a56d59f8d.md)

    The operation to perform when both stencil comparison and depth test passed. 

* [CompareFunction stencil_func](struct_luna_1_1_r_h_i_1_1_depth_stencil_op_desc_1a3473d43f66d2ac9ff3b91f81aa93ed55.md)

    The compare function used for stencil comparison. The comparison is performed between the stencil reference value set by [ICommandBuffer::set_stencil_ref](struct_luna_1_1_r_h_i_1_1_i_command_buffer_1a02299becd77ad76f7ce0e8ebf47003e1.md) and the stencil value in the stencil attachment. 

