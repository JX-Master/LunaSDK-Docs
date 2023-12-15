# Luna::get_processors_count

```c++
LUNA_RUNTIME_API u32 get_processors_count()
```

Gets the number of logical processors on the platform. 

## Overview


## Return value
Returns the number of logical processors on the platform. On hyper-thread machines (Intel/AMD), the number of processors returned will be two times of the physical cores of the CPU. 

