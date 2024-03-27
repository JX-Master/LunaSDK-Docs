# Luna::ShaderCompiler::ShaderCompileResult::entry_point

```c++
Name entry_point
```

The shader entry point function name. 

This should be used instead of [ShaderCompileParameters::entry_point](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters_1a032e067b21a279dbc13d9b1dd9282e5b.md) when specifying entry point in RHI APIs, since the compiler may marshall function names in source files, the entry point name may change before and after compilation. 

