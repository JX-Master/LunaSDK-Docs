# Luna::tls_free

```c++
LUNA_RUNTIME_API void tls_free(opaque_t handle)
```

Frees the TLS slot allocated by `tls_alloc`. 

## Overview
The handle will be invalid after this call and the pointer stored for every thread will be discarded.

Make sure to free all resources bound to the specified slot manually before calling this, or they will never be freed. 

## Parameters
### handle
The handle returned by `tls_alloc`. 

