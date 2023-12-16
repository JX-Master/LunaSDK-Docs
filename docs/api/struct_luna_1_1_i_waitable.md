# Luna::IWaitable
Represents a waitable object used for multi-thread synchronization. 

```c++
interface Luna::IWaitable : public virtual Interface
```

Objects that implements `IWaitable` cannot be used cross process boundary. 

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual void wait()=0](struct_luna_1_1_i_waitable_1a0c78500b6312f13b1d666b30b40fe132.md)

    Waits for this object to be signaled. 

* [virtual bool try_wait()=0](struct_luna_1_1_i_waitable_1a1d4f6f60c080472543ae26b4fa1cc62c.md)

    Tries to wait for this object to be signaled. 

