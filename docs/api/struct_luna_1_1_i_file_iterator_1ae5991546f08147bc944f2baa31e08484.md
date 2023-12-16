# Luna::IFileIterator::get_filename

```c++
virtual const c8 * get_filename()=0
```

Gets the filename of the file that the iterator currently points to. 



## Return value
Returns the name of the file that the iterator currently points to, returns `nullptr` if the file iterator is invalid. The returnd pointer is valid until the file iterator is released or [move_next](struct_luna_1_1_i_file_iterator_1af8a906d9fcf3404a102db1094f874163.md) is called. 

