# Luna::ShaderCompiler::ShaderCompileParameters
Describes one shader compile action. 

```c++
struct Luna::ShaderCompiler::ShaderCompileParameters
```

## Member objects
* [Span<const c8> source](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1abe616ba416cca2bfd033bc2809a00566.md)

    The shader source data in HLSL or GLSL(SPIR-V) format. This is required for one shader compile action. 

* [Name source_name](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a4990cc10bd3d7e8c4cba1e581577ba2a.md)

    The source shader name. This will be used by the compiler and the debug tools to identify the shader if not empty. 

* [Path source_file_path](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1aa56b4a2e68124df0490a8b2637a7cb42.md)

    The platform-native shader source file path. This will be used by the compiler or debugger to resolve local include file and PDB file if not empty. 

* [Name entry_point](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a032e067b21a279dbc13d9b1dd9282e5b.md)

    The entry point function name of the shader. This must not be empty. 

* [TargetFormat target_format](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a5e29d3fb9766ab0a01ec63afc0f7aa08.md)

    The shader compile target format. If the target is [TargetFormat::none](group___shader_compiler_1gga4cad2b3eee9b7fe13c80ad2f66885bd2a334c4a4c42fdb79d7ebc3e73b517e6f8.md), no shader compilation is performed. 

* [ShaderType shader_type](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1aa593e4825886e123f5bae82643543c10.md)

    The type of the shader to compile. 

* [ShaderModel shader_model](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a83cb08b911ed627d04e5bf20fa963080.md)

    The shader model used for compiling shaders. 

* [OptimizationLevel optimization_level](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a0d5f1d432c916dbd046f1b6eb6b46b50.md)

    The optimization level used for compiling shaders. 

* [bool debug](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a398527b3e9e358c345c5047b16871957.md)

    Whether to add debug informations to the shader binary. 

* [bool skip_validation](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a501f5201e51696c282db7c03e512ca68.md)

    Whether to skip shader validation. 

* [MatrixPackMode matrix_pack_mode](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1ae8044d265b93a3d41cf8775397c02570.md)

    The matrix pack mode when interpreting matrix data. 

* [Span<const Path> include_paths](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a13da1249d4f9dd20f94562ed6257c4e8.md)

    One array of paths that the compiler will use to find include files. 

* [Span<const Pair<Name, Name> > definitions](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1af267c8675d2abb4fe0a07d935e407d69.md)

    One set of definitions the compiler will use when preprocessing shader files. 

* [MetalPlatform metal_platform](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a0f084e9bfbcbcfb8da4a830c68f7731b.md)

    The target platform for one metal shader. This is used only if `target_format` is [TargetFormat::msl](group___shader_compiler_1gga4cad2b3eee9b7fe13c80ad2f66885bd2a8cf205e11d5eb3c998ac34958304c608.md). 

