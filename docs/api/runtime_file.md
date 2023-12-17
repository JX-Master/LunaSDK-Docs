# Files


## Classes
* [Luna::FileAttribute](struct_luna_1_1_file_attribute.md)
* [Luna::IFile](struct_luna_1_1_i_file.md)
* [Luna::IFileIterator](struct_luna_1_1_i_file_iterator.md)
## Enumerations
* [Luna::FileAttributeFlag](group___runtime_file_1gaabba864469d3eddd3ad511d82a10d2fa.md)

    Represents file binary attributes. 

* [Luna::FileOpenFlag](group___runtime_file_1gaa6e577ca0057e9e199efe810f7876d3d.md)

    Specifies attributes for one file open operation. 

* [Luna::FileCreationMode](group___runtime_file_1ga191cbeed882d989eae99623be3fd60d3.md)

    Specifies file creation mmode. 

* [Luna::FileCopyFlag](group___runtime_file_1ga962b4537444d213445aa995acbfd667b.md)

    Specify attributes for one file copy operation. 

* [Luna::FileMoveFlag](group___runtime_file_1ga1c21e7a50d0ce43bee48a939a2b7ab4b.md)

    Specify attributes for one file move operation. 

## Functions
* [R< Ref< IFile > > open_file(const c8 *path, FileOpenFlag flags, FileCreationMode creation)](group___runtime_file_1gac58018b1b29fb266021f23592cc864e2.md)

    Opens one file. 

* [R< Blob > load_file_data(IFile *file)](group___runtime_file_1gab709b1bf8a06e1a9246b72566789181d.md)

    Returns the data in the specified file as a blob object. 

* [R< FileAttribute > get_file_attribute(const c8 *path)](group___runtime_file_1ga91b8113efb2471820d683bb2cfacdb06.md)

    Gets the file attribute. 

* [RV copy_file(const c8 *from_path, const c8 *to_path, FileCopyFlag flags=FileCopyFlag::none)](group___runtime_file_1gaadaeff79e86e7dedf1ececda9f02e4e8.md)

    Copies the file or directory from the source path to the destination path. 

* [RV move_file(const c8 *from_path, const c8 *to_path, FileMoveFlag flags=FileMoveFlag::none)](group___runtime_file_1ga1e4a037bfade99aee7028bcced878edd.md)

    Moves the file or directory from the source path to the destination path. This call can also be used to rename a file. 

* [RV delete_file(const c8 *file_path)](group___runtime_file_1ga2cd87aeda1bc96a0141f10208ccbf2fb.md)

    Deletes the specified file or directory. 

* [R< Ref< IFileIterator > > open_dir(const c8 *path)](group___runtime_file_1ga7a98d4ebd233ae412f59326e7e51af14.md)

    Creates a file iterator that can be used to iterate all files in the specified directory. 

* [RV create_dir(const c8 *path)](group___runtime_file_1gabb8938ea556e26b6ba025786d0fbfaf9.md)

    Creates one empty directory. 

* [u32 get_current_dir(u32 buffer_length, c8 *buffer)](group___runtime_file_1gaef6a98ebbc81d069386bc889b345774d.md)

    Gets the current working directory path for the underlying system. 

* [RV set_current_dir(const c8 *path)](group___runtime_file_1ga1d1db0602d90a54a2beb1318be009c23.md)

    Sets the current working directory path for the underlying system. The current directory will be set for the process scope. 

* [const c8 * get_process_path()](group___runtime_file_1gab7c97dde34657264bfd5f1c6a6bd3a0d.md)

    Gets the full (absolute) path of the application's executable file. 

