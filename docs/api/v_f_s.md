# VFS
Virtual file system (VFS) module provides a virtual and uniform file system across all platforms, so that the user can use one uniform path and API to open one file on all platforms without caring where the file is actually in. VFS supports user-implemented file system drivers and devices, which allows the file system to be extended to support reading files from zip archives, online server, etc. 

## Topics
* [VFS Errors](v_f_s_error.md)
## Types
* [Luna::VFS::DriverDesc](struct_luna_1_1_v_f_s_1_1_driver_desc.md)

    Describes one virtual file system (VFS) driver. 


## Functions
* [void register_driver(const Name &name, const DriverDesc &desc)](group___v_f_s_1gacf30a2f98e22e6998df7196b05d3d81f.md)

    Registers one new VFS driver to the system. 

* [RV mount(const Name &driver, const c8 *driver_path, const Path &mount_path, typeinfo_t params_type=nullptr, void *params_data=nullptr)](group___v_f_s_1gae1cf8ad449c3f0db2956b7d81eba02a1.md)

    Mounts one virtual file device as one directory in the virtual file system. 

* [RV unmount(const Path &mount_path)](group___v_f_s_1gafccb3343d41bad7189fe6450c7c57b3f.md)

    Unmounts the virtual file device in the mounting directory. 

* [RV remount(const Path &from_path, const Path &to_path)](group___v_f_s_1gac76e0cde4f7b0adf634e8f13c9689215.md)

    Changes the mounting directory of the file device. 

* [R< Ref< IFile > > open_file(const Path &path, FileOpenFlag flags, FileCreationMode creation)](group___v_f_s_1gaddb61460b7215920d8eb3b8f3ff56535.md)

    Opens one file. 

* [R< FileAttribute > get_file_attribute(const Path &path)](group___v_f_s_1ga47bd35e66bb44921ef1b42592b4a952c.md)

    Gets the file or directory attribute. 

* [RV copy_file(const Path &from_path, const Path &to_path, FileCopyFlag flags=FileCopyFlag::none)](group___v_f_s_1ga4846b28a9667108dcdbca7bb6ec887a7.md)

    Copies the file or directory from the source path to the destination path. 

* [RV move_file(const Path &from_path, const Path &to_path, FileMoveFlag flags=FileMoveFlag::none)](group___v_f_s_1gac9714037d8fbd66967b89591f07c9b35.md)

    Moves the file or directory from the source path to the destination path. This call can also be used to rename a file. 

* [RV delete_file(const Path &path)](group___v_f_s_1gad9ede2837363a6e0ab8e0c781d073ed6.md)

    Deletes the specified file. 

* [R< Ref< IFileIterator > > open_dir(const Path &path)](group___v_f_s_1ga5552736c4484f71fa908c6cb461df3ea.md)

    Creates a file iterator that can be used to iterate all files in the specified directory. 

* [RV create_dir(const Path &path)](group___v_f_s_1ga6940b3f49be0a4e5e97431650751dc9a.md)

    Creates one directory. 

* [R< Name > get_native_path(const Path &vfs_path)](group___v_f_s_1ga4cb638a66c1990d7dc439e72f1040c77.md)

    Translates one VFS path to one native driver path. 

* [Name get_platform_filesystem_driver()](group___v_f_s_1gae6967ff8ad08d41d4952515b6980d397.md)

    Gets the name of the VFS driver that maps platform's native file system to vritual file system. 

