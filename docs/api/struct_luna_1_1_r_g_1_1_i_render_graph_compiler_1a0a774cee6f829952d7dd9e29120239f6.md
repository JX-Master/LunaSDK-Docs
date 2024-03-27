# Luna::RG::IRenderGraphCompiler::get_output_resource

```c++
virtual usize get_output_resource(const Name &name)=0
```

Gets the resource ID of one output resource. 



## Parameters
* *in* **name**

    The name of the output resource. 

## Return value
Returns the resource ID of the resource. Returns [INVALID_RESOURCE](group___r_g_1gac4e99541691ddacbcf16df365d5dcd87.md) if the name is not specified as one output resource. 

