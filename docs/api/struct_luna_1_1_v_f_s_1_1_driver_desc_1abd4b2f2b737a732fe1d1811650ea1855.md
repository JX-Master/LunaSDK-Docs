# Luna::VFS::DriverDesc::on_delete_file

```c++
RV(* on_delete_file) (void *driver_data, void *mount_data, const Path &path)
```

Called when [VFS::delete_file](group___v_f_s_1gad9ede2837363a6e0ab8e0c781d073ed6.md) is called on one file that belongs to devices of this driver. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device. 

* *in* **path**

    The path of the file to delete. 

