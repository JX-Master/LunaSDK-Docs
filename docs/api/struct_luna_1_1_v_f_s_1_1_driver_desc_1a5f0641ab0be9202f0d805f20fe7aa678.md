# Luna::VFS::DriverDesc::on_open_dir

```c++
R< Ref< IFileIterator > >(* on_open_dir) (void *driver_data, void *mount_data, const Path &path)
```

Called when [VFS::open_dir](group___v_f_s_1ga5552736c4484f71fa908c6cb461df3ea.md) is called on one directory that belongs to devices of this driver. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **mount_data**

    The mount data returned by [on_mount](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md) for the device. 

* *in* **path**

    The path of the directory to open. 

## Return value
Returns one file iterator used to enumerate files in the opened directory. 

