# Luna::RG::IRenderGraphCompiler::get_resource_desc

```c++
virtual ResourceDesc get_resource_desc(usize resource)=0
```

Gets the resource descriptor of the specified resource. 



## Parameters
* *in* **resource**

    The resource id returned by [get_input_resource](struct_luna_1_1_r_g_1_1_i_render_graph_compiler_1a500985b9fa0e42f26b42493897f81b84.md) or [get_output_resource](struct_luna_1_1_r_g_1_1_i_render_graph_compiler_1a0a774cee6f829952d7dd9e29120239f6.md). 

## Return value
Returns the resource descriptor of the specified resource. 

## Valid Usage
* `resource` must specify one valid resource. 

