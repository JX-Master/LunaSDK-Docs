# Luna::RHI::IQueryHeap
Contains one array of query elements that can be used to query pipeline execution information, such as pixel occlusion, execution time and pipeline statistics. 

```c++
interface Luna::RHI::IQueryHeap : public virtual IDeviceChild
```

## Base type
* [IDeviceChild](struct_luna_1_1_r_h_i_1_1_i_device_child.md)
## Member functions
* [virtual QueryHeapDesc get_desc()=0](struct_luna_1_1_r_h_i_1_1_i_query_heap_1a9a4a4bb7bc6b10368a39bc2e529dffce.md)

    Gets the descriptor of the query heap. 

* [virtual RV get_timestamp_values(u32 index, u32 count, u64 *values)=0](struct_luna_1_1_r_h_i_1_1_i_query_heap_1a7d1d8fc3dfe62cd8fa7321665d86a7e4.md)

    Copies timestamp query results from query heap to the user-provided buffer. 

* [virtual RV get_occlusion_values(u32 index, u32 count, u64 *values)=0](struct_luna_1_1_r_h_i_1_1_i_query_heap_1ac2dfd3e7ba2069b6663c1c3c8a5c6923.md)

    Copies occlusion query results from query heap to the user-provided buffer. 

* [virtual RV get_pipeline_statistics_values(u32 index, u32 count, PipelineStatistics *values)=0](struct_luna_1_1_r_h_i_1_1_i_query_heap_1a7dae7881087e9125ef117c74a0a6e2ec.md)

    Copies pipeline statistics query results from query heap to the user-provided buffer. 

