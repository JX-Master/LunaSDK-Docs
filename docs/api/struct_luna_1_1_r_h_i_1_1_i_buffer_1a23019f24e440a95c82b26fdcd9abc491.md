# Luna::RHI::IBuffer::map

```c++
virtual RV map(usize read_begin, usize read_end, void **data)=0
```

Maps the resource data to system memory and enables CPU access to the resource data. Map/unmap operations are reference counted, for each `map` operation, you need to call `unmap` once to finally unmap the memory. 



## Parameters
* *in* **read_begin**

    The offset, in bytes, of the beginning of the data range that will be read by CPU. 

* *in* **read_end**

    The offset, in bytes, of the ending of the data range that will be read by CPU. 

* *out* **data**

    Returns the pointer to the mapped memory. The returned pointer is not offsetted by `read_begin` and always points to the beginning of the resource data, but only data in [pointer + read_begin, pointer + read_end) range is valid for reading from CPU.


If `read_end <= read_begin`, no data will be read by CPU, which is required if resource heap type is not `MemoryType::readback`.

If `read_end` is larger than the subresource size (like setting to `USIZE_MAX`), the read range will be clamped to [read_begin, resource_size). 

