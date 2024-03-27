# Luna::RHI::ICommandBuffer::draw_indexed_instanced

```c++
virtual void draw_indexed_instanced(u32 index_count_per_instance, u32 instance_count, u32 start_index_location, i32 base_vertex_location, u32 start_instance_location)=0
```

Draws indexed, instanced primitives. 



## Parameters
* *in* **index_count_per_instance**

    The number of indices to draw for every instance. 

* *in* **instance_count**

    The number of instances to draw. 

* *in* **start_index_location**

    The position of the index pointing to first per-vertex data to use for instance drawing. Vertex data pointed by index in range [`start_index_location`, `start_index_location + index_count_per_instance`) will be used. 

* *in* **base_vertex_location**

    An offset that will be added to all indices numbers before dereferring vertex data from their indices. This can be used to batch vertices of multiple meshes into one vertex buffer, and use offsets to draw each of them separately. 

* *in* **start_instance_location**

    The index of the first per-instance data to use for instance drawing. Instance data in range [`start_instance_location`, `start_instance_location + instance_count`) will be used. 

