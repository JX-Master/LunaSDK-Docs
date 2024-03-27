# Luna::RHI::ICommandBuffer::copy_resource

```c++
virtual void copy_resource(IResource *dst, IResource *src)=0
```

Copies the entire contents of the source resource to the destination resource. 



## Parameters
* *in* **dst**

    The resource to copy data to. 

* *in* **src**

    The resource to copy data from. 

## Valid Usage
* The source resource and destination resource must have exactly the same resource format and dimension, that is, have the same size for buffers, or the same type, width, height, depth, format, mip count, array count and sample count for textures. 

