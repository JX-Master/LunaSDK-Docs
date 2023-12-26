# Luna::UniquePtr::release

```c++
pointer release()
```

Sets the native pointer to null, and gets the original pointer. 



## Return value
Returns the original pointer wrapped by this smart pointer. The returned pointer may be `nullptr` if the smart pointer is null when this function is called. 

