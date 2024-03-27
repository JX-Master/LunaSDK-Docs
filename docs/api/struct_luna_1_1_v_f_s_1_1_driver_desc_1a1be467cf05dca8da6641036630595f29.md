# Luna::VFS::DriverDesc::on_unmount

```c++
RV(* on_unmount) (void *driver_data, void *mount_data)
```

Called when one device is unmounted. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md). 

