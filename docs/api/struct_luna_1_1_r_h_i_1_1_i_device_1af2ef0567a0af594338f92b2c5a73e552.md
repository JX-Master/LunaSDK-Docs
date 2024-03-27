# Luna::RHI::IDevice::new_texture

```c++
virtual R< Ref< ITexture > > new_texture(MemoryType memory_type, const TextureDesc &desc, const ClearValue *optimized_clear_value=nullptr)=0
```

Creates one new texture resource and allocates device memory for the resource. 



## Parameters
* *in* **memory_type**

    The memory type selected for allocating resource memory. 

* *in* **desc**

    The descriptor object. 

* *in* **optimized_clear_value**

    The optional optimized clear value for a texture resource. Specify `nullptr` if the resource does not have a optimized clear value. 

## Return value
Returns the created texture object. 

