# Luna::RHI::ShaderVisibilityFlag

```c++
enum ShaderVisibilityFlag : u8
{
    vertex= 0x01
    pixel= 0x02
    compute= 0x04
    all= vertex | pixel | compute
}
```

Specifies which shader can access descriptors in the specified binding. 

## Options
* [vertex](group___r_h_i_1gga4dfc1279e665f25cb66d7bcfacfb796fa2b5bc093b09bd81f51de433bde9d202a.md)

    The vertex shader can access descriptors in the specified binding. 

* [pixel](group___r_h_i_1gga4dfc1279e665f25cb66d7bcfacfb796faab4086ecd47c568d5ba5739d4078988f.md)

    The pixel shader can access descriptors in the specified binding. 

* [compute](group___r_h_i_1gga4dfc1279e665f25cb66d7bcfacfb796fa77e73f3a185e16d1f08ca5e057710b9d.md)

    The compute shader can access descriptors in the specified binding. 

* [all](group___r_h_i_1gga4dfc1279e665f25cb66d7bcfacfb796faa181a603769c1f98ad927e7367c7aa51.md)

    All shaders can access descriptors in the specified binding. 

