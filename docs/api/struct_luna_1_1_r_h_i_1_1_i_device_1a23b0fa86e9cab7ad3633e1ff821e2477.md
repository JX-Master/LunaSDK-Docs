# Luna::RHI::IDevice::new_buffer

```c++
virtual R< Ref< IBuffer > > new_buffer(MemoryType memory_type, const BufferDesc &desc)=0
```

Creates one new buffer resource and allocates device memory for the resource. 



## Parameters
* *in* **memory_type**

    The memory type selected for allocating resource memory. 

* *in* **desc**

    The descriptor object. 

## Return value
Returns the created buffer object. 

