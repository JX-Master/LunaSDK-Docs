# Luna::VFS::DriverDesc::on_get_file_attribute

```c++
R< FileAttribute >(* on_get_file_attribute) (void *driver_data, void *mount_data, const Path &path)
```

Called when [VFS::get_file_attribute](group___v_f_s_1ga47bd35e66bb44921ef1b42592b4a952c.md) is called on one file or directory belongs to one device of this driver. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device. 

* *in* **path**

    The path of the file or directory to check relative to the mount root path. 

## Return value
Returns the file attribute object. 

