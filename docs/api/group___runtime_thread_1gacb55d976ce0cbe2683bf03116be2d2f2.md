# Luna::tls_set

```c++
void tls_set(opaque_t handle, void *ptr)
```

Set the data bound to the current thread's TLS slot specified by `handle`. 



## Parameters
* *in* **handle**

    The handle of the slot specified. The handle must be allocated first by `tls_alloc`. 

* *in* **ptr**

    The pointer value to set to this slot. 

