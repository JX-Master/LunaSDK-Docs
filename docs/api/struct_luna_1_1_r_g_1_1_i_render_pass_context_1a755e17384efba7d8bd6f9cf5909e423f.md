# Luna::RG::IRenderPassContext::get_timestamp_query_heap

```c++
virtual RHI::IQueryHeap * get_timestamp_query_heap(u32 *begin_index, u32 *end_index)=0
```

Gets the timestamp query heap used to track the running time of the render pass. 



## Parameters
* *out* **begin_index**

    If not `nullptr`, returns the query heap index to write the beginning timestamp of the render pass. 

* *out* **end_index**

    If not `nullptr`, returns the query heap index to write the ending timestamp of the render pass. 

## Return value
Returns the timestamp query heap used to track the running time of the render pass. Returns `nullptr` if timestamp query is not used in this render graph ( [RenderGraphCompileConfig::enable_time_profiling](struct_luna_1_1_r_g_1_1_render_graph_compile_config_1a6ae73fbc722d8cd8db973c9bf600fcb5.md) is `false`). 

