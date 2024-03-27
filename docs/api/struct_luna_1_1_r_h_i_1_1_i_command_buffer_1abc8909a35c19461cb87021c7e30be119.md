# Luna::RHI::ICommandBuffer::set_vertex_buffers

```c++
virtual void set_vertex_buffers(u32 start_slot, Span< const VertexBufferView > views)=0
```

Sets vertex buffers. 



## Parameters
* *in* **start_slot**

    The start slot of the vertex buffer to set. 

* *in* **views**

    An array of vertex buffer views to set, each describes one vertex buffer range to bind. The vertex buffer views will be set in slot [start_slot, start_slot + views.size()). 

