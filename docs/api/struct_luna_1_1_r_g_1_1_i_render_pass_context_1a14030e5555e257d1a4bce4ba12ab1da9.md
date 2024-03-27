# Luna::RG::IRenderPassContext::get_output

```c++
virtual RHI::IResource * get_output(const Name &name)=0
```

Gets the output resource of the render pass. 



## Parameters
* *in* **name**

    The name of the output resource. 

## Return value
Returns the fetched output resource. Returns `nullptr` if not found. 

