# Luna::RHI::ICommandBuffer::begin_copy_pass

```c++
virtual void begin_copy_pass(const CopyPassDesc &desc=CopyPassDesc())=0
```

Begins a copy pass. 

The following functions can only be called in between `begin_copy_pass` and `end_copy_pass`:* copy_resource

* copy_buffer

* copy_texture

* copy_buffer_to_texture

* copy_texture_to_buffer 

## Parameters
* *in* **desc**

    The copy pass descriptor. 

