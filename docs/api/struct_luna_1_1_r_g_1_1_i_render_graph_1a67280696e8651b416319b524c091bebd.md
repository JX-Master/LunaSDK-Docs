# Luna::RG::IRenderGraph::get_pass_time_intervals

```c++
virtual RV get_pass_time_intervals(Vector< u64 > &pass_times)=0
```

Gets the time used for every active render pass. 



## Parameters
* *out* **pass_times**

    The array to receive the elapsed time for every active render pass. The size of this array is the same as the size of the array returned by [get_enabled_render_passes](struct_luna_1_1_r_g_1_1_i_render_graph_1ade3e5438b0a2dc5f563042a799a96b55.md), and every time span in this array maps to the corresponding render pass returned by [get_enabled_render_passes](struct_luna_1_1_r_g_1_1_i_render_graph_1ade3e5438b0a2dc5f563042a799a96b55.md). The time is measured in GPU ticks, and can be converted to seconds by dividing with [RHI::IDevice::get_command_queue_timestamp_frequency](struct_luna_1_1_r_h_i_1_1_i_device_1ac868409c6ccfb1010f64373db0f0235d.md). 

