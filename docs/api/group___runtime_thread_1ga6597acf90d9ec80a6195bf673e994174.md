# Luna::tls_get

```c++
void * tls_get(opaque_t handle)
```

Get the value bound to the TLS slot of current thread. 



## Parameters
### handle
The handle of the slot to query. 

## Return value
Returns the pointer set, or `nullptr` if no pointer is set to this slot. 

