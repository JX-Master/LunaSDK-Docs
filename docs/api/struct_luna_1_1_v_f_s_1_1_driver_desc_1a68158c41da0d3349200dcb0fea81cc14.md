# Luna::VFS::DriverDesc::on_get_native_path

```c++
R< Name >(* on_get_native_path) (void *driver_data, void *mount_data, const Path &path)
```

Called when [VFS::get_native_path](group___v_f_s_1ga4cb638a66c1990d7dc439e72f1040c77.md) is called on one path that belongs to devices of this driver. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device. 

* *in* **path**

    The path to convert. 

## Return value
Returns one path string that represents the converted native path. 

