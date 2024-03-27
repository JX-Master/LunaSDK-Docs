# Luna::RHI::IDeviceChild
Represents one object that is created by [IDevice](struct_luna_1_1_r_h_i_1_1_i_device.md) and is only available in the device context. 

```c++
interface Luna::RHI::IDeviceChild : public virtual Interface
```

Every device child object holds one strong reference to the devices that creates it, so the device object will not be destroyed until all device child objects are destroyed. 

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual IDevice * get_device()=0](struct_luna_1_1_r_h_i_1_1_i_device_child_1a4d3ba9e434cf51eaf322a54629f22a12.md)

    Gets the device that creates this object. 

* [virtual void set_name(const c8 *name)=0](struct_luna_1_1_r_h_i_1_1_i_device_child_1a1cc3e3da9668281b43162800a5d012a8.md)

    Sets the name of the device object. This name is for use in debug diagnostics and tools. 

