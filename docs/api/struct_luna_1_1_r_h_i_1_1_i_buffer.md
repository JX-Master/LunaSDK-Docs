# Luna::RHI::IBuffer
Represents one buffer resource that can be used to contain arbitrary binary data. 

```c++
interface Luna::RHI::IBuffer : public virtual IResource
```

## Base type
* [IResource](struct_luna_1_1_r_h_i_1_1_i_resource.md)
## Member functions
* [virtual BufferDesc get_desc()=0](struct_luna_1_1_r_h_i_1_1_i_buffer_1ad0f429f6f4ab5065767e043a360562c7.md)

    Gets the descriptor of this buffer object. 

* [virtual RV map(usize read_begin, usize read_end, void **data)=0](struct_luna_1_1_r_h_i_1_1_i_buffer_1a23019f24e440a95c82b26fdcd9abc491.md)

    Maps the resource data to system memory and enables CPU access to the resource data. Map/unmap operations are reference counted, for each `map` operation, you need to call `unmap` once to finally unmap the memory. 

* [virtual void unmap(usize write_begin, usize write_end)=0](struct_luna_1_1_r_h_i_1_1_i_buffer_1af2767ed8d8df249817bb0c85cfecf6f0.md)

    Invalidates the pointer to the mapped data, and synchronizes changed data with device when needed. Map/unmap operations are reference counted, for each `map` operation, you need to call `unmap` once to finally unmap the memory. 

