# Luna::RHI::ICommandBuffer::draw

```c++
virtual void draw(u32 vertex_count, u32 start_vertex_location)=0
```

Draw primitives. 



## Parameters
* *in* **vertex_count**

    The number of vertices to draw. 

* *in* **start_vertex_location**

    The position of the first vertex to draw. Vertices in range [`start_vertex_location`, `start_vertex_location + vertex_count`) will be drawn. 

