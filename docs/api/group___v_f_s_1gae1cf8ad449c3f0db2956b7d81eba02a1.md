# Luna::VFS::mount

```c++
RV mount(const Name &driver, const c8 *driver_path, const Path &mount_path, typeinfo_t params_type=nullptr, void *params_data=nullptr)
```

Mounts one virtual file device as one directory in the virtual file system. 



## Parameters
* *in* **driver**

    The name of the VFS driver for the virtual file device. 

* *in* **driver_path**

    The path passed to the driver, which is usually the native path mapped to the mount path. 

* *in* **mount_path**

    The directory used as the root directory of the mounted file device. 

* *in* **params_type**

    The type of the additional driver parameter object. See driver docs for details. 

* *in* **params_data**

    The pointer to the additional driver parameter object. See driver docs for details. 

