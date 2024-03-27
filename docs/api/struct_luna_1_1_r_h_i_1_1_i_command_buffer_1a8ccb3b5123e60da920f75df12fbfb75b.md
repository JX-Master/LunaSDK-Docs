# Luna::RHI::ICommandBuffer::attach_device_object

```c++
virtual void attach_device_object(IDeviceChild *obj)=0
```

Attaches one graphic device object to this command buffer. The command buffer keeps a strong reference to the object until the next `reset` is called. 

This is mainly used to keep references to the graphic objects used by the current command buffer, so they will not be released before GPU finishes accessing them. 

