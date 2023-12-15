# Luna::IFileIterator
Represents a directory stream that can be used to iterate all files and directories in the specified directory. See open_dir for details. 

```c++
interface Luna::IFileIterator : public virtual Interface
```

## Functions
* [virtual bool is_valid()=0](struct_luna_1_1_i_file_iterator_1a8ad5b340ebf155189dae99f009494ff5.md)

    Checks if this iterator points to a valid file in the directory stream. 

* [virtual const c8 * get_filename()=0](struct_luna_1_1_i_file_iterator_1ae5991546f08147bc944f2baa31e08484.md)

    Gets the filename of the file that the iterator currently points to. 

* [virtual FileAttributeFlag get_attributes()=0](struct_luna_1_1_i_file_iterator_1afd5c25f51fb0dc06d6009c2e14a1f204.md)

    Gets the file attribute flags of the file. 

* [virtual bool move_next()=0](struct_luna_1_1_i_file_iterator_1af8a906d9fcf3404a102db1094f874163.md)

    Moves the iterator to the next file in the directory. 

