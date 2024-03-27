# Luna::RHI::IDevice::get_command_queue_desc

```c++
virtual CommandQueueDesc get_command_queue_desc(u32 command_queue_index)=0
```

Gets the command queue descriptor of the specified command queue. 



## Parameters
* *in* **command_queue_index**

    The index of the command queue to check. 

## Return value
Returns the command queue descriptor of the specified command queue. 

## Valid Usage
* `command_queue_index` must be in range [`0`, `get_num_command_queues()`). 

