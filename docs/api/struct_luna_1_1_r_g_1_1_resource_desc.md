# Luna::RG::ResourceDesc
Describes one render graph resource. 

```c++
struct Luna::RG::ResourceDesc
```

## Member objects
* [ResourceType type](struct_luna_1_1_r_g_1_1_resource_desc_1a4a108db1de35312357266a380d24cdab.md)

    The resource type. 

* [RHI::MemoryType memory_type](struct_luna_1_1_r_g_1_1_resource_desc_1a78d857b2947067986b8a70ea666d584d.md)

    The resource memory type. 

* [RHI::BufferDesc buffer](struct_luna_1_1_r_g_1_1_resource_desc_1aa0cdacb3cd6a86f931fed6ed9d820751.md)

    Describes the resource if `type` is [ResourceType::buffer](group___r_g_1gga3a2bffc4475e3d9654bfdd8a5dad771aa7f2db423a49b305459147332fb01cf87.md). 

* [RHI::TextureDesc texture](struct_luna_1_1_r_g_1_1_resource_desc_1ae9feaeb4ef7aff70c62d02658f804218.md)

    Describes the resource if `type` is [ResourceType::texture](group___r_g_1gga3a2bffc4475e3d9654bfdd8a5dad771aa6d788fcb39cecfd54da7b065a8b75d1a.md). 

