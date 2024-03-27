# Shader Compiler
The ShaderCompiler module provides API to compile shaders. ShaderCompiler is designed to work with RHI, but it can also be used independently to implement shader compile command-line tools without importing RHI module. 

## Types
* [Luna::ShaderCompiler::ShaderModel](struct_luna_1_1_shader_compiler_1_1_shader_model.md)

    Specifies the HLSL shader model version used when compiling HLSL source code. 


* [Luna::ShaderCompiler::ShaderCompileParameters](struct_luna_1_1_shader_compiler_1_1_shader_compile_parameters.md)

    Describes one shader compile action. 


* [Luna::ShaderCompiler::ShaderCompileResult](struct_luna_1_1_shader_compiler_1_1_shader_compile_result.md)

    Describes shader compile result. 


* [Luna::ShaderCompiler::ICompiler](struct_luna_1_1_shader_compiler_1_1_i_compiler.md)

    The compiler that compiles one shader source code into one target form. 


## Enumerations
* [Luna::ShaderCompiler::TargetFormat](group___shader_compiler_1ga4cad2b3eee9b7fe13c80ad2f66885bd2.md)

    The compile target to output. 

* [Luna::ShaderCompiler::MatrixPackMode](group___shader_compiler_1ga5664501f890659bca1cece4835bda8f8.md)

    The matrix pack mode. 

* [Luna::ShaderCompiler::ShaderType](group___shader_compiler_1gabf3bb737d635d8642abed505ec38053f.md)

    Specifies the shader compile type. 

* [Luna::ShaderCompiler::OptimizationLevel](group___shader_compiler_1gad0d1a1a53d57ad777cab9b18439e571a.md)

    Specifies the shader optimization level. 

* [Luna::ShaderCompiler::MetalPlatform](group___shader_compiler_1gacb74be69dafe7a2290c1f7fd6dae9fd3.md)

    Specifies the intended running platform for one metal shader. 

## Functions
* [Ref< ICompiler > new_compiler()](group___shader_compiler_1ga01ef6d3c5abeed3e5b6766f53fcefff6.md)

    Creates one new compiler. 

