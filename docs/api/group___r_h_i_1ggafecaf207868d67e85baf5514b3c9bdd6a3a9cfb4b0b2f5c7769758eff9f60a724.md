# Luna::RHI::ResourceFlag::allow_aliasing

```c++
allow_aliasing = 0x01
```

Specify this flag will allow multiple resources sharing the same memory with this resource. If this flag is not set when calling `new_buffer` or `new_texture`, the memory allocated along with the resource cannot be used for creating another resource by calling `new_aliasing_buffer` or `new_aliasing_texture`. 

This flag is ignored and will be set for new resources created with `new_aliasing_buffer` or `new_aliasing_texture`, since such resources are always aliased. 

