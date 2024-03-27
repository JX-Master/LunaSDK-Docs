# Luna::RG::RenderGraphResourceType

```c++
enum RenderGraphResourceType : u8
{
    transient= 0
    persistent= 1
    external= 2
}
```

Specifies the residency type of one resource in one render graph. 

## Options
* [transient](group___r_g_1ggae76da9a01d229922ee38eb0efec5b857af15455eb297257c3414c2e6959a92e60.md)

    This resource is used to hold temporal data during the render graph execution. The render graph allocates this resource at first access, and releases the resource after last access. 

* [persistent](group___r_g_1ggae76da9a01d229922ee38eb0efec5b857a23c6323bfb57bb630b8a2ecf703d6bb0.md)

    This resource is persistent. Such resources are used to hold data between render graph executions. The render graph allocates this resource when the graph is being compiled, and does not release it after the render graph execution is finished. 

* [external](group___r_g_1ggae76da9a01d229922ee38eb0efec5b857a6a21b6995a068148bbb65c8f949b3fb2.md)

    This resource is imported to the render graph. The render graph does not manage the resource lifetime. 

