# Luna::RHI::IDevice::new_swap_chain

```c++
virtual R< Ref< ISwapChain > > new_swap_chain(u32 command_queue_index, Window::IWindow *window, const SwapChainDesc &desc)=0
```

Creates one swap chain and binds it to the specified window. 



## Parameters
* *in* **command_queue_index**

    The command queue attached to the swap chain. Present commands will only be submitted to the command queue attached with the swap chain. 

* *in* **window**

    The window that the new swap chain should be bound to. 

* *in* **desc**

    The swap chain descriptor object. 

## Return value
Returns the new created swap chain object. 

## Valid Usage
* `command_queue_index` must be in range [`0`, `get_num_command_queues()`).

* The swap chain specified by `command_queue_index` must have [CommandQueueFlag::presenting](group___r_h_i_1ggaaa41659a673405f1b0553989ed7bc8eda1c0350bade516fb53180f02d26e6064e.md) being set. 

