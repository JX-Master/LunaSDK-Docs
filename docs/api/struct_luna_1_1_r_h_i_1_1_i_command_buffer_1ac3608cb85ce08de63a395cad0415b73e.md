# Luna::RHI::ICommandBuffer::draw_indexed

```c++
virtual void draw_indexed(u32 index_count, u32 start_index_location, i32 base_vertex_location)=0
```

Draw indexed primitives. 



## Parameters
* *in* **index_count**

    The number of indices to draw. 

* *in* **start_index_location**

    The position of the first index to draw. Indices in range [`start_index_location`, `start_index_location + index_count`) will be drawn. 

* *in* **base_vertex_location**

    An offset that will be added to all indices numbers before dereferring vertex data from their indices. This can be used to batch vertices of multiple meshes into one vertex buffer, and use offsets to draw each of them separately. 

