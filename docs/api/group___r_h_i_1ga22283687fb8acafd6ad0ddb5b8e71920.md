# Luna::RHI::BufferUsageFlag

```c++
enum BufferUsageFlag : u16
{
    copy_source= 0x01
    copy_dest= 0x02
    uniform_buffer= 0x04
    read_buffer= 0x08
    read_write_buffer= 0x10
    vertex_buffer= 0x20
    index_buffer= 0x40
    indirect_buffer= 0x80
}
```

Specifies possible usages for one [IBuffer](struct_luna_1_1_r_h_i_1_1_i_buffer.md) object. 

## Options
* [copy_source](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a751fdad2b83af8ed443d3c2d6efd7822.md)

    Allows this resource to be bound as copy source. 

* [copy_dest](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a3a20bc63470d18df9ac2b7163b5d89f6.md)

    Allows this resource to be bound as copy destination. 

* [uniform_buffer](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a9e3ed97709be98ed347af4bbf765daec.md)

    Allows this resource to be bound to a uniform buffer view. 

* [read_buffer](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a4a5ac64bedcfb6cf9b0228d787f81ce2.md)

    Allows this resource to be bound to a read buffer view. 

* [read_write_buffer](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a0e51440a37396d4e0444a6f77ed2f2b3.md)

    Allows this resource to be bound to a read-write buffer view. 

* [vertex_buffer](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a9a89a832efcc2557585b289cc295f7f5.md)

    Allows this resource to be bound as a vertex buffer. 

* [index_buffer](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920aab150dddbaa3966d354cc6dcd7418ea9.md)

    Allows this resource to be bound as a index buffer. 

* [indirect_buffer](group___r_h_i_1gga22283687fb8acafd6ad0ddb5b8e71920a6c1d372277c0e5dbef946d0f5a7fb1ee.md)

    Allows this resource to be bound as a buffer providing indirect draw arguments. 

