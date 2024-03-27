# Luna::RHI::ICommandBuffer::resource_barrier

```c++
virtual void resource_barrier(Span< const BufferBarrier > buffer_barriers, Span< const TextureBarrier > texture_barriers)=0
```

Issues one resource barrier that synchronizes GPU pipeline access to multiple resources. 



## Parameters
* *in* **buffer_barriers**

    The buffer barriers to submitl. 

* *in* **texture_barriers**

    The texture barriers to submit. 

