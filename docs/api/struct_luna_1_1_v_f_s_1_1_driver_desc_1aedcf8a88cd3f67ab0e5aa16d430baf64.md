# Luna::VFS::DriverDesc::on_mount

```c++
R< void * >(* on_mount) (void *driver_data, const c8 *driver_path, const Path &mount_dir, typeinfo_t params_type, void *params_data)
```

Called when one new device is mounted. 



## Parameters
* *in* **driver_data**

    The user-provided driver data. 

* *in* **driver_path**

    The driver native path passed to [mount](group___v_f_s_1gae1cf8ad449c3f0db2956b7d81eba02a1.md). 

* *in* **mount_dir**

    The directory used as the root directory of the mounted file device. 

* *in* **params_type**

    The type of the additional driver parameter object passed to [mount](group___v_f_s_1gae1cf8ad449c3f0db2956b7d81eba02a1.md). 

* *in* **params_data**

    The pointer to the additional driver parameter object passed to [mount](group___v_f_s_1gae1cf8ad449c3f0db2956b7d81eba02a1.md). 

## Return value
Returns the mount data that identifies the mounted device. 

