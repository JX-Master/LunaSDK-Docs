# Luna::RHI::IBuffer::unmap

```c++
virtual void unmap(usize write_begin, usize write_end)=0
```

Invalidates the pointer to the mapped data, and synchronizes changed data with device when needed. Map/unmap operations are reference counted, for each `map` operation, you need to call `unmap` once to finally unmap the memory. 



## Parameters
* *in* **write_begin**

    The offset, in bytes, of the beginning of the data range that is changed by CPU and should be synchronized. 

* *in* **write_end**

    The offset, in bytes, of the ending of the data range that is changed by CPU and should be synchronized.


If `write_begin <= write_end`, no data will be synchronized, which is required if resource heap type is not `MemoryType::upload`.

If `write_end` is larger than the subresource size (like setting to `USIZE_MAX`), the write range will be clamped to [write_begin, resource_size). 

