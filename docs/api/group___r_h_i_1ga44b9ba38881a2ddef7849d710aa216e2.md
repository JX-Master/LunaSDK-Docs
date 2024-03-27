# Luna::RHI::DescriptorType

```c++
enum DescriptorType : u8
{
    uniform_buffer_view
    read_buffer_view
    read_write_buffer_view
    read_texture_view
    read_write_texture_view
    sampler
}
```

Specifies the type of descriptors that can be placed in a descriptor set. 

## Options
* [uniform_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a34a06ac1c4c09077554ac744585760a8.md)

    Specifies uniform buffer view, which allows reading data from one uniform buffer. This descriptor is supported in all shaders. 

* [read_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a6a92853feaf697b82bc7a540363df626.md)

    Specifies read buffer view, which allows reading data from one structured buffer. This descriptor is supported in all shaders. 

* [read_write_buffer_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2ac803981c38618413594fc9655c788c01.md)

    Speciifes read-write buffer view, which allows reading and writing data from one structured buffer. This descriptor is supported in compute shader only. 

* [read_texture_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2aceda36ce0ea7592cd04d237493431753.md)

    Specifies read texture view, which allows reading texture data using pixel coordinates directly or sampling texture data from the texture using samplers. This descriptor is supported in all shaders. 

* [read_write_texture_view](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2aff0f72f27c8460d323630827e870a1ba.md)

    Specifies read-write texture view, which allows reading and writing texture data using pixel coordinates directly. This descriptor is supported in compute shader only. 

* [sampler](group___r_h_i_1gga44b9ba38881a2ddef7849d710aa216e2a2b06a2251d39e28f8220696766dcd136.md)

    Specifies one sampler. This descriptor is supported in all shaders. 

