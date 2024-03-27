# Luna::RHI::ComputePipelineStateDesc::pipeline_layout

```c++
IPipelineLayout* pipeline_layout
```

The pipeline layout used with this pipeline state. 

This is used to check the compatibility between the pipeline layout and the pipeline state when creating the pipeline state object. Depends the implementation, the pipeline state object may or may not stores one refernce to this pipeline layout. When binding pipeline layouts and pipeline states to pipelines, any pipeline layout that is compatible to this pipeline state can be used. 

