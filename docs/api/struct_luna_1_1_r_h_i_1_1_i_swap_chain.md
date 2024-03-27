# Luna::RHI::ISwapChain
Represents one swap chain used for presenting images to the screen. 

```c++
interface Luna::RHI::ISwapChain : public virtual IDeviceChild
```

## Base type
* [IDeviceChild](struct_luna_1_1_r_h_i_1_1_i_device_child.md)
## Member functions
* [virtual Window::IWindow * get_window()=0](struct_luna_1_1_r_h_i_1_1_i_swap_chain_1a6263fef0f6d3bbb87f296f92542da146.md)

    Gets the window that this swap chain bounds to. 

* [virtual SwapChainDesc get_desc()=0](struct_luna_1_1_r_h_i_1_1_i_swap_chain_1addb5a132009e208b60bb20adb33203b5.md)

    Gets the descriptor object. 

* [virtual R< ITexture * > get_current_back_buffer()=0](struct_luna_1_1_r_h_i_1_1_i_swap_chain_1a515a4bdcf361219dc63856bd21db0541.md)

    Gets the current back buffer that is available for rendering. 

* [virtual RV present()=0](struct_luna_1_1_r_h_i_1_1_i_swap_chain_1abb083503b72d6df1a5d3065434c225e8.md)

    Submits the current back buffer to the bounding queue for presenting. 

* [virtual RV reset(const SwapChainDesc &desc)=0](struct_luna_1_1_r_h_i_1_1_i_swap_chain_1a2d75908cf2d1b8faf4f0251bc93bf05b.md)

    Resets the swap chain. 

