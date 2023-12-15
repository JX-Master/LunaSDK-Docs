# Luna::load_file_data

```c++
LUNA_RUNTIME_API R< Blob > load_file_data(IFile *file)
```

Returns the data in the specified file as a blob object. 

## Overview


## Parameters
### file
The file to read. 

## Return value
Returns the data of the file. 

#### Valid Usage
* `file` must be opened with FileOpenFlag::read flag. 

