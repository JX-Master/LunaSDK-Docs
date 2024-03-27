# Luna::RHI::IDevice::get_command_queue_timestamp_frequency

```c++
virtual R< f64 > get_command_queue_timestamp_frequency(u32 command_queue_index)=0
```

Gets the GPU timestamp frequency of the specified command queue. The timestamp frequency is measured in ticks per second. 



## Parameters
* *in* **command_queue_index**

    The index of the command queue to check. 

## Return value
Returns the GPU timestamp frequency of the specified command queue. 

## Valid Usage
* `command_queue_index` must be in range [`0`, `get_num_command_queues()`). 

