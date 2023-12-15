# Luna::yield_current_thread

```c++
LUNA_RUNTIME_API void yield_current_thread()
```

Yields the remain time slice of the current thread and let OS to schedule other threads. 

## Overview
There is no way to resume a thread from user mode, since threads are scheduled by OS automatically. 

