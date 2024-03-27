# Luna::RG::IRenderGraph::compile

```c++
virtual RV compile(const RenderGraphCompileConfig &config)=0
```

Compiles the render graph. 

This function does the following steps in order:1. Set up internal render pass and resource data.

1. Cull out unused passes and resources by scanning all dependency render passes and resources of output resources.

1. Determines the lifetime of every transient resource.

1. Initialize resource descriptors using user-defined descriptors.

1. Calls the compile callback of every render pass in execution order to get render pass objects.

1. Create persistent resources.

1. Create time query heap if needed. 

## Parameters
* *in* **config**

    The compilation configuration. 

