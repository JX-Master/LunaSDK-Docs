# Luna::RG::IRenderGraph::get_persistent_resource

```c++
virtual RHI::IResource * get_persistent_resource(usize index)=0
```

Gets one persistent resource. 



## Parameters
* *in* **index**

    The index of the resource to get. 

## Return value
Returns the persistent resource of the specified index. Returns `nullptr` if the index is not valid or does not specify one persistent resource. 

