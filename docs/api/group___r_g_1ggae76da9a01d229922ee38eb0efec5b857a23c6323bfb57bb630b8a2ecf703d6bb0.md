# Luna::RG::RenderGraphResourceType::persistent

```c++
persistent = 1
```

This resource is persistent. Such resources are used to hold data between render graph executions. The render graph allocates this resource when the graph is being compiled, and does not release it after the render graph execution is finished. 

This resource will be released when the render graph is destructed or recompiled. 

