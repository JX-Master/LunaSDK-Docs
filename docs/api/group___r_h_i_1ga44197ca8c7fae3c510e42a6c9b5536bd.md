# Luna::RHI::BufferStateFlag

```c++
enum BufferStateFlag : u32
{
    none= 0x00
    indirect_argument= 0x01
    vertex_buffer= 0x02
    index_buffer= 0x04
    uniform_buffer_vs= 0x08
    shader_read_vs= 0x10
    uniform_buffer_ps= 0x20
    shader_read_ps= 0x40
    shader_write_ps= 0x80
    uniform_buffer_cs= 0x0100
    shader_read_cs= 0x0200
    shader_write_cs= 0x0400
    copy_dest= 0x0800
    copy_source= 0x1000
    automatic= 0x80000000
    shader_read_write_ps= shader_read_ps | shader_write_ps
    shader_read_write_cs= shader_read_cs | shader_write_cs
}
```

Specifies buffer resource states before and after one barrier. 

## Options
* [none](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda334c4a4c42fdb79d7ebc3e73b517e6f8.md)

    This resource is not used by the pipeline. Resources with no state flag cannot be used by the pipeline, and must be transfered to one valid state before it can be used. 

* [indirect_argument](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda5ac04f676f3f586a3d0be24f3294622d.md)

    Used as a indirect argument buffer. 

* [vertex_buffer](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda9a89a832efcc2557585b289cc295f7f5.md)

    Used as a vertex buffer. 

* [index_buffer](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdaab150dddbaa3966d354cc6dcd7418ea9.md)

    Used as a index buffer. 

* [uniform_buffer_vs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdab2ebf68d6b62a10bd85214636bd31ca9.md)

    Used as a uniform buffer for vertex shader. 

* [shader_read_vs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdae41f0d10766049d8cd369a7a766554b7.md)

    Used as a read-only resource for vertex shader. 

* [uniform_buffer_ps](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda1884af2fc4e5298451f0043fc79b0cd2.md)

    Used as a uniform buffer for pixel shader. 

* [shader_read_ps](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda920178b8787f75d9b60d3886edd9ad17.md)

    Used as a read-only resource for pixel shader. 

* [shader_write_ps](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdaecaddf3df743e0d38ec9cf9852fcf55d.md)

    Used as a write-only resource for pixel shader. Enabled only if pixel shader write feature is supported. 

* [uniform_buffer_cs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda7f8b735a63524a2131db6c6a4f610db4.md)

    Used as a uniform buffer for compute shader. 

* [shader_read_cs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda3d2c8dfbaeefb3364d0fce53d56ecb9f.md)

    Used as a read-only resource for compute shader. 

* [shader_write_cs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda3ecff0025edf0eef76ebe5b48d29c7fb.md)

    Used as a write-only resource for compute shader. 

* [copy_dest](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda3a20bc63470d18df9ac2b7163b5d89f6.md)

    Used as a copy destination. 

* [copy_source](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda751fdad2b83af8ed443d3c2d6efd7822.md)

    Used as a copy source. 

* [automatic](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda2bd9c0ed00116be1258e0cc66617d7c8.md)

    If this is specified as the before state, the system determines the before state automatically using the last state specified in the same command buffer for the resource. If this is the first time the resource is used in the current command buffer, the system loads the resource's global state automatically. 

* [shader_read_write_ps](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdae4043ca5437c0888e2df1fe9a3583550.md)

    Used as a read-write resource for pixel shader. This is a combination of [shader_read_ps](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda920178b8787f75d9b60d3886edd9ad17.md) and [shader_write_ps](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdaecaddf3df743e0d38ec9cf9852fcf55d.md). 

* [shader_read_write_cs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bdaf67c9a9e770113c836391887ed6e63c3.md)

    Used as a read-write resource for compute shader. This is a combination of [shader_read_cs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda3d2c8dfbaeefb3364d0fce53d56ecb9f.md) and [shader_write_cs](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda3ecff0025edf0eef76ebe5b48d29c7fb.md). 

