# Luna::VFS::DriverDesc::on_driver_unregister

```c++
void(* on_driver_unregister) (void *driver_data)
```

Called when the driver is unregistered from VFS. 

The user should release all dynamic memory attached to [driver_data](struct_luna_1_1_v_f_s_1_1_driver_desc_1a4a210b06acf4842476c0308219d7ced9.md) if any. 

## Parameters
* *in* **driver_data**

    The user-provided driver data. 

