# Luna::RHI::IDevice::allocate_memory

```c++
virtual R< Ref< IDeviceMemory > > allocate_memory(MemoryType memory_type, Span< const BufferDesc > buffers, Span< const TextureDesc > textures)=0
```

Allocates device memory that is capable of storing resources specified. 



## Parameters
* *in* **memory_type**

    The memory type of the memory to allocate. 

* *in* **buffers**

    One array of descriptors of buffers that once the allocation succeeds, can be created in the memory. 

* *in* **textures**

    One array of descriptors of textures that once the allocation succeeds, can be created in the memory. 

## Return value
Returns the allocated memory. 

