# Luna::fast_sleep

```c++
void fast_sleep(u32 time_microseconds)
```

Delays the execution of this thread for a very shout time by yielding this thread several times. 

This is more accurate to `sleep` method and will not suspend current thread unless the specified time is larger than several milliseconds. 

## Parameters
* *in* **time_microseconds**

    The time, in microseconds, that this thread needs to delay. 

