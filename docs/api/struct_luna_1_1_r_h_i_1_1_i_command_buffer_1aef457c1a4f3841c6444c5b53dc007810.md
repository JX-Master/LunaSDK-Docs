# Luna::RHI::ICommandBuffer::begin_compute_pass

```c++
virtual void begin_compute_pass(const ComputePassDesc &desc=ComputePassDesc())=0
```

Begins a compute pass. 

The following functions can only be called in between `begin_compute_pass` and `end_compute_pass`:* set_compute_pipeline_layout

* set_compute_pipeline_state

* set_compute_descriptor_set

* set_compute_descriptor_sets

* dispatch 

## Parameters
* *in* **desc**

    The compute pass descriptor. 

