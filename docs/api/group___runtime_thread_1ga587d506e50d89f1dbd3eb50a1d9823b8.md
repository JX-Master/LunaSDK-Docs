# Luna::new_thread

```c++
LUNA_RUNTIME_API Ref< IThread > new_thread(void(*entry_func)(void *params), void *params, const c8 *name=nullptr, u32 stack_size=0)
```

Create a new system thread and make it run the callback function. The thread will be closed when the callback function returns. 

## Overview


## Parameters
### entry_func
The function to invoke by the new thread. 

### params
The additional parameter passed to the callback. 

### name
The name of the thread. This is usually for debug purpose. 

### stack_size
The stack size for new thread's call stack. 

## Return value
Returns an interface representing the new created thread. 

