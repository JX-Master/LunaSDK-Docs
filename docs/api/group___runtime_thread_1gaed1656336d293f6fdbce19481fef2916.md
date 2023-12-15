# Luna::tls_alloc

```c++
LUNA_RUNTIME_API opaque_t tls_alloc(tls_destructor *destructor=nullptr)
```

Allocates one thread local storage (TLS) slot. 

## Overview
The TLS slot is allocated for every thread running in this process, including the thread that is currently not being created yet. After the handle is returned, every thread can set a thread-local value to this slot using this handle.

The allocated slot is large enough to store one pointer to the real thread-local data. The pointer is `nullptr` for every thread before it is firstly modified by that thread. 

## Parameters
### destructor
The optional destructor to use for this TLS slot. If this is not `nullptr`, this destructor will be called on one thread when that thread exits and the TLS pointer value of this slot for that thread is not `nullptr`.


When the destructor is called, the system resets the TLS value to `nullptr` and passes the original TLS value to the destructor. This process may be repeated several times until the TLS value is `nullptr` after the destructor returns.

## Return value
Returns the handle to the TLS slot. 

