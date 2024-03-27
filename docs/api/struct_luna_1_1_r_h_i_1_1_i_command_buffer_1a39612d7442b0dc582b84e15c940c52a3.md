# Luna::RHI::ICommandBuffer::reset

```c++
virtual RV reset()=0
```

Resets the command buffer. This call clears all commands in the command buffer, resets the state tracking infrastructure and reopens the command buffer for recording new commands. 

You should only call this after the command buffer has finished execution by the command queue, or the behavior is undefined. In order to make sure all commands are executed by GPU, call `wait` to block the thread until this buffer gets finished, or you can use `try_wait` to test if the buffer has finished execution. 

