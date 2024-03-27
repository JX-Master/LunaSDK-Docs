# Luna::RHI::ICommandBuffer::dispatch

```c++
virtual void dispatch(u32 thread_group_count_x, u32 thread_group_count_y, u32 thread_group_count_z)=0
```

Dispatches one compute task. 



## Parameters
* *in* **thread_group_count_x**

    The number of thread groups to emit in the first dimension. 

* *in* **thread_group_count_y**

    The number of thread groups to emit in the second dimension. 

* *in* **thread_group_count_z**

    The number of thread groups to emit in the third dimension. 

