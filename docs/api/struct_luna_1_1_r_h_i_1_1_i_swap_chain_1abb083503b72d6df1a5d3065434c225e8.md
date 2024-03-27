# Luna::RHI::ISwapChain::present

```c++
virtual RV present()=0
```

Submits the current back buffer to the bounding queue for presenting. 



## Remark
This function only enqueues the presentation command to the command queue and returns immediately after the command is successfully enqueued. The user must ensure that all writes to the current back buffer is completed before calling `present` to present the back buffer. 

