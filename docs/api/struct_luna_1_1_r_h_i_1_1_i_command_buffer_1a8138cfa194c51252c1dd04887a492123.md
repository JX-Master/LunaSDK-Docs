# Luna::RHI::ICommandBuffer::begin_occlusion_query

```c++
virtual void begin_occlusion_query(OcclusionQueryMode mode, u32 index)=0
```

Starts one occlusion query. 



## Parameters
* *in* **mode**

    The working mode of the new occlusion query. 

* *in* **index**

    The position to write occlusion query result to. Multiple occlusion queries can exist at the same time, so long as each of them takes one separate index. 

