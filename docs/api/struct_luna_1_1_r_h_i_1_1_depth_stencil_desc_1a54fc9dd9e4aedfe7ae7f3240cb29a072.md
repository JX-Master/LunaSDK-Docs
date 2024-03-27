# Luna::RHI::DepthStencilDesc::stencil_read_mask

```c++
u8 stencil_read_mask
```

The mask used to specify bits that will be loaded from stencil buffer for stencil testing. All bits that are not specified in the mask (with mask bit value 0) will be set to 0 before stencil testing is performed. 

