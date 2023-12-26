# Luna::ISemaphore
Represents one system-level semaphore object. 

```c++
interface Luna::ISemaphore : public virtual IWaitable
```

## Base type
* [IWaitable](struct_luna_1_1_i_waitable.md)
## Member functions
* [virtual void release()=0](struct_luna_1_1_i_semaphore_1aab0a52fdd148a54108e7bf49287d7c47.md)

    Increases the counter value of the semaphore by one. 

