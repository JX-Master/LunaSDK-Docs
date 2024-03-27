# Luna::RHI::ICommandBuffer::copy_buffer

```c++
virtual void copy_buffer(IBuffer *dst, u64 dst_offset, IBuffer *src, u64 src_offset, u64 copy_bytes)=0
```

Copies buffer data region from one buffer to another. 



## Parameters
* *in* **dst**

    The buffer to copy data to. 

* *in* **dst_offset**

    The offset, in bytes, of the first data byte to copy data to in `dst`. 

* *in* **src**

    The buffer to copy data from. 

* *in* **src_offset**

    The offset, in bytes, of the first data byte to copy data from to in `src`. 

* *in* **copy_bytes**

    The number of bytes to copy. 

