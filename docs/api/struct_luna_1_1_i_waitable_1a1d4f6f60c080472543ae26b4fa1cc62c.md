# Luna::IWaitable::try_wait

```c++
virtual bool try_wait()=0
```

Tries to wait for this object to be signaled. 

This will not suspend the current thread, if the condition is not satisfied, this call returns immediately with `false`. 

