# Luna::RHI::IDevice::new_aliasing_texture

```c++
virtual R< Ref< ITexture > > new_aliasing_texture(IDeviceMemory *device_memory, const TextureDesc &desc, const ClearValue *optimized_clear_value=nullptr)=0
```

Creates one aliasing texture that shares the same device memory with the existing resource. 

The user may create multiple aliasing resources with the same device memory, given that only one of them is active at any given time. The user should use aliasing barrier to switch the active resource between aliasing resources sharing the same device memory. 

## Parameters
* *in* **device_memory**

    The device memory that the new resource is created in. 

* *in* **desc**

    The descriptor object. 

* *in* **optimized_clear_value**

    The optional optimized clear value for a texture resource. Specify `nullptr` if the resource does not have a optimized clear value. 

## Return value
Returns the created texture object. 

