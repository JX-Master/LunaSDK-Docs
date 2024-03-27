# Luna::RHI::ResourceFlag

```c++
enum ResourceFlag : u16
{
    allow_aliasing= 0x01
}
```

Specifies additional flags for one resource. 

## Options
* [allow_aliasing](group___r_h_i_1ggafecaf207868d67e85baf5514b3c9bdd6a3a9cfb4b0b2f5c7769758eff9f60a724.md)

    Specify this flag will allow multiple resources sharing the same memory with this resource. If this flag is not set when calling `new_buffer` or `new_texture`, the memory allocated along with the resource cannot be used for creating another resource by calling `new_aliasing_buffer` or `new_aliasing_texture`. 

