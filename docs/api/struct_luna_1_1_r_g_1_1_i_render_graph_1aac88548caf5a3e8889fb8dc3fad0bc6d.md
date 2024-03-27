# Luna::RG::IRenderGraph::set_external_resource

```c++
virtual void set_external_resource(usize index, RHI::IResource *resource)=0
```

Sets external resource. 

Since external resources are not allocated and managed by the render graph, they must be set explicitly before executing the render graph. 

## Parameters
* *in* **index**

    The index of the resource to set. 

* *in* **resource**

    The resource to set. 

## Valid Usage
* `index` must specify one resource with [RenderGraphResourceType::external](group___r_g_1ggae76da9a01d229922ee38eb0efec5b857a6a21b6995a068148bbb65c8f949b3fb2.md). 

