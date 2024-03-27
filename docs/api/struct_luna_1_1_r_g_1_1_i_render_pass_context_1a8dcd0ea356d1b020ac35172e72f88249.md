# Luna::RG::IRenderPassContext::get_input

```c++
virtual RHI::IResource * get_input(const Name &name)=0
```

Gets the input resource of the render pass. 



## Parameters
* *in* **name**

    The name of the input resource. 

## Return value
Returns the fetched input resource. Returns `nullptr` if not found. 

