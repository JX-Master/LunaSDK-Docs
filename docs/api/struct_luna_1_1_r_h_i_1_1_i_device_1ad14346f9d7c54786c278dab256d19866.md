# Luna::RHI::IDevice::is_resources_aliasing_compatible

```c++
virtual bool is_resources_aliasing_compatible(MemoryType memory_type, Span< const BufferDesc > buffers, Span< const TextureDesc > textures)=0
```

Checks whether the given resources can share the same device memory. 

This can be used to check whether the specified resources can be allocated from the same device memory without actually allocating such memory. 

## Parameters
* *in* **memory_type**

    The memory type for the given buffers and textures. 

* *in* **buffers**

    The buffer descriptors of resources being examined. 

* *in* **textures**

    The texture descriptors of resources being examined. 

## Return value
Returns `true` if such resources can share the same device memory, returns `false` otherwise. 

