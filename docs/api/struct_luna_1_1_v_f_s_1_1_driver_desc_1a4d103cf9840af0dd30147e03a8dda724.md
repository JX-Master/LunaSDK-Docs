# Luna::VFS::DriverDesc::on_move_file

```c++
RV(* on_move_file) (void *driver_data, void *from_mount_data, void *to_mount_data, const Path &from_path, const Path &to_path, FileMoveFlag flags)
```

Called when [VFS::move_file](group___v_f_s_1gac9714037d8fbd66967b89591f07c9b35.md) is called on two files that both belong to devices of this driver. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **from_mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device that the file is moved from. 

* *in* **to_mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device that the file is moved to. 

* *in* **from_path**

    The path of the file to move from relative to the mount root path. 

* *in* **to_path**

    The path of the file to move to relative to the mount root path. 

* *in* **flags**

    The file move flags. 

