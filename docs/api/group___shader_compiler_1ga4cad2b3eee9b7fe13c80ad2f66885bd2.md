# Luna::ShaderCompiler::TargetFormat

```c++
enum TargetFormat : u8
{
    none= 0
    dxil
    spir_v
    msl
}
```

The compile target to output. 

## Options
* [none](group___shader_compiler_1gga4cad2b3eee9b7fe13c80ad2f66885bd2a334c4a4c42fdb79d7ebc3e73b517e6f8.md)

    Outputs nothing. This can be used if you only want to validate the input source code. 

* [dxil](group___shader_compiler_1gga4cad2b3eee9b7fe13c80ad2f66885bd2ab1c1dc1e21cc6036396f949afce779c6.md)

    [Windows only] Outputs DirectX Intermediate Language for shader model 6.0 and newer. 

* [spir_v](group___shader_compiler_1gga4cad2b3eee9b7fe13c80ad2f66885bd2a4e01b95158a0dd8ab3941df67f4c6774.md)

    Outputs SPIR-V for Vulkan API. 

* [msl](group___shader_compiler_1gga4cad2b3eee9b7fe13c80ad2f66885bd2a8cf205e11d5eb3c998ac34958304c608.md)

    Outputs Metal Shading Lauguage. 

