# Luna::tls_free

```c++
void tls_free(opaque_t handle)
```

Frees the TLS slot allocated by `tls_alloc`. 

The handle will be invalid after this call and the pointer stored for every thread will be discarded.

Make sure to free all resources bound to the specified slot manually before calling this, or they will never be freed. 

## Parameters
### handle
The handle returned by `tls_alloc`. 

## Remark
Note that calling `tls_free` will not call the destructor registered for this slot on any thread. After `tls_free` is called, the destructor will be cleared and will not be called any more. 

