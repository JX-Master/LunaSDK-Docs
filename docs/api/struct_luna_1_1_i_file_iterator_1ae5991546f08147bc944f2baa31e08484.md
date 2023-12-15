# Luna::IFileIterator::get_filename

```c++
virtual const c8 * get_filename()=0
```

Gets the filename of the file that the iterator currently points to. 

## Overview


## Return value
Returns the name of the file that the iterator currently points to, returns `nullptr` if the file iterator is invalid. The returnd pointer is valid until the file iterator is released or move_next is called. 

