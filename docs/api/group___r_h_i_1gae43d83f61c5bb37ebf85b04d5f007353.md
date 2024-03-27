# Luna::RHI::ResourceDataCopyOp

```c++
enum ResourceDataCopyOp : u8
{
    read_buffer
    write_buffer
    read_texture
    write_texture
}
```

Specifies the type of one resource data copy operation. 

## Options
* [read_buffer](group___r_h_i_1ggae43d83f61c5bb37ebf85b04d5f007353a4a5ac64bedcfb6cf9b0228d787f81ce2.md)

    Copy data of one buffer resource from resource memory to host memory. 

* [write_buffer](group___r_h_i_1ggae43d83f61c5bb37ebf85b04d5f007353a1ef7c725bfb35a78474778ab93cd001f.md)

    Copy data of one buffer resource from host memory to resource memory. 

* [read_texture](group___r_h_i_1ggae43d83f61c5bb37ebf85b04d5f007353a4d21c382c71b7e96839d30e304a6b755.md)

    Copy data of one texture resource from resource memory to host memory. 

* [write_texture](group___r_h_i_1ggae43d83f61c5bb37ebf85b04d5f007353a6c87ab538e5211e5c28688e6beab9363.md)

    Copy data of one texture resource from host memory to resource memory. 

