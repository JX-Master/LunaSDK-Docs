# Luna::RHI::IDevice::new_aliasing_buffer

```c++
virtual R< Ref< IBuffer > > new_aliasing_buffer(IDeviceMemory *device_memory, const BufferDesc &desc)=0
```

Creates one aliasing buffer that shares the same device memory with the existing resource. 

The user may create multiple aliasing resources with the same device memory, given that only one of them is active at any given time. The user should use aliasing barrier to switch the active resource between aliasing resources sharing the same device memory. 

## Parameters
* *in* **device_memory**

    The device memory that the new resource is created in. 

* *in* **desc**

    The descriptor object. 

## Return value
Returns the created buffer object. 

