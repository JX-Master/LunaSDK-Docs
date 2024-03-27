# Luna::VFS::DriverDesc::on_copy_file

```c++
RV(* on_copy_file) (void *driver_data, void *from_mount_data, void *to_mount_data, const Path &from_path, const Path &to_path, FileCopyFlag flags)
```

Called when [VFS::copy_file](group___v_f_s_1ga4846b28a9667108dcdbca7bb6ec887a7.md) is called on two files that both belong to devices of this driver. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **from_mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device that the file is copied from. 

* *in* **to_mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device that the file is copied to. 

* *in* **from_path**

    The path of the file to copy from relative to the mount root path. 

* *in* **to_path**

    The path of the file to copy to relative to the mount root path. 

* *in* **flags**

    The file copy flags. 

