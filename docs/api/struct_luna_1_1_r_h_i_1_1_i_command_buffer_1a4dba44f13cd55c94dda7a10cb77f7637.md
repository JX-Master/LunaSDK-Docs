# Luna::RHI::ICommandBuffer::draw_instanced

```c++
virtual void draw_instanced(u32 vertex_count_per_instance, u32 instance_count, u32 start_vertex_location, u32 start_instance_location)=0
```

Draws non-indexed, instanced primitives. 



## Parameters
* *in* **vertex_count_per_instance**

    The number of vertices to draw for every instance. 

* *in* **instance_count**

    The number of instances to draw. 

* *in* **start_vertex_location**

    The position of the first per-vertex data to use for instance drawing. Vertex data in range [`start_vertex_location`, `start_vertex_location + vertex_count_per_instance`) will be used. 

* *in* **start_instance_location**

    The index of the first per-instance data to use for instance drawing. Instance data in range [`start_instance_location`, `start_instance_location + instance_count`) will be used. 

