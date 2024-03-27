# Luna::RHI::ComputePassDesc
Describes one compute pass. 

```c++
struct Luna::RHI::ComputePassDesc
```

## Member objects
* [IQueryHeap* timestamp_query_heap](struct_luna_1_1_r_h_i_1_1_compute_pass_desc_1ad8f257d32b9f8609cae0973c09b61dfc.md)

    The timestamp query heap that the query data will be written to if not `nullptr`. 

* [IQueryHeap* pipeline_statistics_query_heap](struct_luna_1_1_r_h_i_1_1_compute_pass_desc_1af73b3b78911a849e97de8795f33476a3.md)

    The pipeline statistics query heap that the query data will be written to if not `nullptr`. 

* [u32 timestamp_query_begin_pass_write_index](struct_luna_1_1_r_h_i_1_1_compute_pass_desc_1abdce645223cefbb19c950af746cbd2eb.md)

    The index of the element in timestamp query heap that the compute pass begin timestamp will be written to. If this is [DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md), the query data will not be written. 

* [u32 timestamp_query_end_pass_write_index](struct_luna_1_1_r_h_i_1_1_compute_pass_desc_1a8852fe8f6016604273236959c8f2af78.md)

    The index of the element in timestamp query heap that the compute pass end timestamp will be written to. If this is [DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md), the query data will not be written. 

* [u32 pipeline_statistics_query_write_index](struct_luna_1_1_r_h_i_1_1_compute_pass_desc_1aab659b8951b9eea11f8ec237e202aaf1.md)

    The index of the element in pipeline statistics query heap that the pipeline statistics will be written to. If this is [DONT_QUERY](group___r_h_i_1ga2d53aab2964919c53d15e5769fb6dd63.md), the query data will not be written. 

