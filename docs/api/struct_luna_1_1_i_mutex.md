# Luna::IMutex
This\ type\ is\ thread\ safe. Represents a system-level mutex object. 

```c++
interface Luna::IMutex : public virtual IWaitable
```

The mutex or critical section is an important object that provides synchronization functionality for multiple threads that wants to access the same resource without data race. The mutex can be "owned" by at most one thread, when other threads wants to acquire the mutex, it must wait until the thread that currently owns the mutex to release the mutex. The threads that waits on the mutex will probably be suspended by system.

The mutex can be acquired recursively, that is, the thread that already owns the mutex can make additional calls to acquire the mutex, so long as it makes one release call for each acquire call to finally release the mutex.

Acquiring the mutex from one thread and releasing from another thread is not allowed. 

## Base type
* [IWaitable](struct_luna_1_1_i_waitable.md)
## Member functions
* [virtual void unlock()=0](struct_luna_1_1_i_mutex_1a31262d17e02fcf1524984b10d72dee3e.md)

    Releases the ownership of the mutex. 

