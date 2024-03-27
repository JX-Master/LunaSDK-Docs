# Luna::RHI::ISwapChain::get_current_back_buffer

```c++
virtual R< ITexture * > get_current_back_buffer()=0
```

Gets the current back buffer that is available for rendering. 



## Return value
Returns the current back buffer that is available for rendering. 

## Remark
The first call to `get_current_back_buffer` after `present` may block the current thread until at least one back buffer is available for rendering, or until an error occurs. After the first successful `get_current_back_buffer` call, all succeeding calls to `get_current_back_buffer` return the same back buffer until another `present` call is issued. Every `present` call evicts the user access to the current back buffer, and next `get_current_back_buffer` call will wait for another back buffer available for rendering. The returned back buffer resource should be released immediately after `present` is called. 

