# Luna::RHI::SwapChainDesc
Describes one swap chain. 

```c++
struct Luna::RHI::SwapChainDesc
```

## Member objects
* [u32 width](struct_luna_1_1_r_h_i_1_1_swap_chain_desc_1a85db88ffee2944ecd35c616393976289.md)

    The width of the swap chain back buffer. Specify 0 will determine the size from the bounding window's native size. 

* [u32 height](struct_luna_1_1_r_h_i_1_1_swap_chain_desc_1add40f8a56ae8cc650f92a3aa4d2bac99.md)

    The width of the swap chain back buffer. Specify 0 will determine the size from the bounding window's native size. 

* [u32 buffer_count](struct_luna_1_1_r_h_i_1_1_swap_chain_desc_1a6a69429caeb3049e92250c747d5c8f6e.md)

    The number of back buffers in the swap chain. 

* [Format format](struct_luna_1_1_r_h_i_1_1_swap_chain_desc_1a751c4987b2c6908c70a915ab18d36653.md)

    The pixel format of the back buffer. 

* [bool vertical_synchronized](struct_luna_1_1_r_h_i_1_1_swap_chain_desc_1a142e9e30faa6e6ce1d3ce2f6f490e87f.md)

    Whether to synchronize frame image presentation to vertical blanks of the monitor. 

