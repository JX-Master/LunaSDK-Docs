# Luna::RHI::ICommandBuffer::submit

```c++
virtual RV submit(Span< IFence * > wait_fences, Span< IFence * > signal_fences, bool allow_host_waiting)=0
```

Submits the recorded commands in this command buffer to the attached command queue. 

The command buffer can only be submitted once, and the only allowed operation after submit is to reset the command buffer after it is executed by command queue. 

## Parameters
* *in* **wait_fences**

    The fence objects to wait before this command buffer can be processed by the system. 

* *in* **signal_fences**

    The fence objects to signal after this command buffer is completed. 

* *in* **allow_host_waiting**

    Whether [ICommandBuffer::wait](struct_luna_1_1_i_waitable_1a0c78500b6312f13b1d666b30b40fe132.md) can be used to wait for the command buffer from host side. If this is `false`, the command buffer cannot be waited from host, and the behavior of calling [ICommandBuffer::wait](struct_luna_1_1_i_waitable_1a0c78500b6312f13b1d666b30b40fe132.md) is undefined. Setting this to `false` may improve queue performance, and the command buffer can still be waited by other command buffers using fences.

## Remark
Command buffers submitted to the same command queue are processed by their submission order without overlapping, so that one command buffer will not be executed until all previous command buffers in the same command queue are completely finished, and their writes are made visible to this command buffer.


If `signal_fences` is not empty, the system guarantees that all commands in the submission is finished, and all writes to the memory in the submission is made visible before fences are signaled. 

