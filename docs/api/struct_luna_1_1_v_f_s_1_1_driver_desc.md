# Luna::VFS::DriverDesc
Describes one virtual file system (VFS) driver. 

```c++
struct Luna::VFS::DriverDesc
```

One VFS driver describes functions to operate files on a certain kind of media. For example, one ZIP driver may provide functions to read files from one ZIP archive, and the file devices created from the driver represents one real ZIP file opened for reading. 

## Member objects
* [void* driver_data](struct_luna_1_1_v_f_s_1_1_driver_desc_1a4a210b06acf4842476c0308219d7ced9.md)

    The user-defined driver data pointer that will be passed to all driver callback functions. 

* [void(* on_driver_unregister) (void *driver_data)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a2c3861d5e39c706fd7bcde42b1ce7af2.md)

    Called when the driver is unregistered from VFS. 

* [R< void * >(* on_mount) (void *driver_data, const c8 *driver_path, const Path &mount_dir, typeinfo_t params_type, void *params_data)](struct_luna_1_1_v_f_s_1_1_driver_desc_1aedcf8a88cd3f67ab0e5aa16d430baf64.md)

    Called when one new device is mounted. 

* [RV(* on_unmount) (void *driver_data, void *mount_data)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a1be467cf05dca8da6641036630595f29.md)

    Called when one device is unmounted. 

* [R< Ref< IFile > >(* on_open_file) (void *driver_data, void *mount_data, const Path &path, FileOpenFlag flags, FileCreationMode creation)](struct_luna_1_1_v_f_s_1_1_driver_desc_1ae8b4dfb424afc86b8b4c131a3dd9f3c6.md)

    Called when [VFS::open_file](group___v_f_s_1gaddb61460b7215920d8eb3b8f3ff56535.md) is called on one file or directory belongs to one device of this driver. 

* [R< FileAttribute >(* on_get_file_attribute) (void *driver_data, void *mount_data, const Path &path)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a16a9dce5bc8448095dd9e119a0073001.md)

    Called when [VFS::get_file_attribute](group___v_f_s_1ga47bd35e66bb44921ef1b42592b4a952c.md) is called on one file or directory belongs to one device of this driver. 

* [RV(* on_copy_file) (void *driver_data, void *from_mount_data, void *to_mount_data, const Path &from_path, const Path &to_path, FileCopyFlag flags)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a9b512849ba9e77a9db7ec300e50abc52.md)

    Called when [VFS::copy_file](group___v_f_s_1ga4846b28a9667108dcdbca7bb6ec887a7.md) is called on two files that both belong to devices of this driver. 

* [RV(* on_move_file) (void *driver_data, void *from_mount_data, void *to_mount_data, const Path &from_path, const Path &to_path, FileMoveFlag flags)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a4d103cf9840af0dd30147e03a8dda724.md)

    Called when [VFS::move_file](group___v_f_s_1gac9714037d8fbd66967b89591f07c9b35.md) is called on two files that both belong to devices of this driver. 

* [RV(* on_delete_file) (void *driver_data, void *mount_data, const Path &path)](struct_luna_1_1_v_f_s_1_1_driver_desc_1abd4b2f2b737a732fe1d1811650ea1855.md)

    Called when [VFS::delete_file](group___v_f_s_1gad9ede2837363a6e0ab8e0c781d073ed6.md) is called on one file that belongs to devices of this driver. 

* [R< Ref< IFileIterator > >(* on_open_dir) (void *driver_data, void *mount_data, const Path &path)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a5f0641ab0be9202f0d805f20fe7aa678.md)

    Called when [VFS::open_dir](group___v_f_s_1ga5552736c4484f71fa908c6cb461df3ea.md) is called on one directory that belongs to devices of this driver. 

* [RV(* on_create_dir) (void *driver_data, void *mount_data, const Path &path)](struct_luna_1_1_v_f_s_1_1_driver_desc_1abe73711ca1896e4e1f02ccb2e0dc3b0a.md)

    Called when [VFS::create_dir](group___v_f_s_1ga6940b3f49be0a4e5e97431650751dc9a.md) is called on one directory that belongs to devices of this driver. 

* [R< Name >(* on_get_native_path) (void *driver_data, void *mount_data, const Path &path)](struct_luna_1_1_v_f_s_1_1_driver_desc_1a68158c41da0d3349200dcb0fea81cc14.md)

    Called when [VFS::get_native_path](group___v_f_s_1ga4cb638a66c1990d7dc439e72f1040c77.md) is called on one path that belongs to devices of this driver. 

