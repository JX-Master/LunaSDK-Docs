# Luna::RHI::IDevice::new_command_buffer

```c++
virtual R< Ref< ICommandBuffer > > new_command_buffer(u32 command_queue_index)=0
```

Creates one command buffer. 



## Parameters
* *in* **command_queue_index**

    The index of the command queue that will be attached to the command buffer. The command buffer can only submit commands to its attached command queue. 

## Return value
Returns the created command buffer object. 

## Valid Usage
* `command_queue_index` must be in range [`0`, `get_num_command_queues()`). 

