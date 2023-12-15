# Files


## Classes
* [Luna::FileAttribute](struct_luna_1_1_file_attribute.md)
* [Luna::IFile](struct_luna_1_1_i_file.md)
* [Luna::IFileIterator](struct_luna_1_1_i_file_iterator.md)
## Functions
* [LUNA_RUNTIME_API R< Ref< IFile > > open_file(const c8 *path, FileOpenFlag flags, FileCreationMode creation)](group___runtime_file_1ga9c6802285bfe5d9b47a067487cfb665c.md)

    Opens one file. 

* [LUNA_RUNTIME_API R< Blob > load_file_data(IFile *file)](group___runtime_file_1ga5db366dac73029877752fb2969d767ec.md)

    Returns the data in the specified file as a blob object. 

* [LUNA_RUNTIME_API R< FileAttribute > get_file_attribute(const c8 *path)](group___runtime_file_1gafc817765c2a5febb456d0d0728685295.md)

    Gets the file attribute. 

* [LUNA_RUNTIME_API RV copy_file(const c8 *from_path, const c8 *to_path, FileCopyFlag flags=FileCopyFlag::none)](group___runtime_file_1ga403fdc9a5e3d0192d169112ab09937c3.md)

    Copies the file or directory from the source path to the destination path. 

* [LUNA_RUNTIME_API RV move_file(const c8 *from_path, const c8 *to_path, FileMoveFlag flags=FileMoveFlag::none)](group___runtime_file_1gacd11152f82d27b7d4edaead28e0056c0.md)

    Moves the file or directory from the source path to the destination path. This call can also be used to rename a file. 

* [LUNA_RUNTIME_API RV delete_file(const c8 *file_path)](group___runtime_file_1gadf474a92aea43a8fc8d0a494545b4166.md)

    Deletes the specified file or directory. 

* [LUNA_RUNTIME_API R< Ref< IFileIterator > > open_dir(const c8 *path)](group___runtime_file_1ga34fd3952c7f15f22c272f9d4e568436d.md)

    Creates a file iterator that can be used to iterate all files in the specified directory. 

* [LUNA_RUNTIME_API RV create_dir(const c8 *path)](group___runtime_file_1ga88c4a1aee80b54bcc1c6220f64151028.md)

    Creates one empty directory. 

* [LUNA_RUNTIME_API u32 get_current_dir(u32 buffer_length, c8 *buffer)](group___runtime_file_1gaf2b20ca5fdbac9bed29388cb94d4a68a.md)

    Gets the current working directory path for the underlying system. 

* [LUNA_RUNTIME_API RV set_current_dir(const c8 *path)](group___runtime_file_1gae7531a6ee8352538200ef1502d2dedc2.md)

    Sets the current working directory path for the underlying system. The current directory will be set for the process scope. 

* [LUNA_RUNTIME_API const c8 * get_process_path()](group___runtime_file_1gac78ec88a75597d9ed708a7e53109de15.md)

    Gets the full (absolute) path of the application's executable file. 

